---
layout: single
title: "조건문"
toc: true
toc_sticky: true
toc_label: "페이지 주요 목차"
---

### 01. 책 구입하기
![책구입](/assets/images/책구입.PNG)

~~~c
#include <stdio.h>
int main() {
  int money, remain, book=15000;

  printf("money: ");
  scanf("%d", &money);
  
  if(money>=book){
    remain=money-book;
    printf("책 구입 성공!\n나머지: %d", remain);
  }else
    printf("책 구입 실패!");
  return 0;
  }
~~~
  
  ### 02. 도어락 해제하기
  ![도어락](/assets/images/도어락.PNG)
  
~~~c
 #include <stdio.h>
 int main() {
  int select;
  char dic='c', ic;
  int dpw=24680, pw;
  double dfin=1.2345678, fin;

  printf("select: ");
  scanf("%d", &select);

  if (select==1){
    printf("IC: ");
    scanf(" %c", &ic);
  }else if (select==2){
    printf("password: ");
    scanf("%d", &pw);
  }else{
    printf("finger: ");
    scanf("%lf", &fin);
  }
  
  if(dic==ic || dpw==pw || dfin==fin)
    printf("문 열림~");
  else
    printf("디리릭!디리릭!");
    return 0;
   }
~~~
   
   ### 03. 가위바위보
   ![가위바위보](/assets/images/가위바위보.PNG)
   
~~~c
   #include <stdio.h>
 int main() {
    char com, user;
    com='r';
    printf("r/s/p: ");
    scanf("%c", &user);
    
    if(com==user)
    printf("비겼다")
    else if((user=='r' && com=='s')||(suer='s'&&com=='p')||(user=='p'&&com=='r'))
      printf("이겼다");
    else
      printf("졌다")

      return 0;
      }
~~~

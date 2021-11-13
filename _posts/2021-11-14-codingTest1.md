---
layout: post
title: 짝수와 홀수
categories: 프로그래머스
author: Sowon Park
tags: [programers,codingTest,C]
date: 2021-11-14 07:41 +0800
---
## Level 1
### 정수 num이 짝수일 경우 "Even"을 반환하고 홀수인 경우 "Odd"를 반환하는 함수, solution을 완성해주세요.
**제한 조건**
> num은 int 범위의 정수입니다.  
> 0은 짝수입니다.

**사용언어 C**  

```c
#include <stdio.h>
#include <stdbool.h>
#include <stdlib.h>

char* solution(int num) {
    // 리턴할 값은 메모리를 동적 할당해주세요
    char* answer = (char*)malloc(sizeof(char)*num);
    if (num%2!=0)   answer = "Odd"; 
    // num이 2로 나누어 떨어지지 않으면 홀수이므로 answer에 "Odd" 값 할당
    else            answer = "Even";
    return answer;
}

int main(){
    printf("%s",solution(3));
    // "Odd"
    return 0;
}
```

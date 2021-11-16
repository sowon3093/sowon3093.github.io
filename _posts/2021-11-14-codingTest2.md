---
layout: post
title: 정수 내림차순으로 배치하기
categories: Python
author: Sowon Park
tags: [programers,codingTest,Python]
date: 2021-11-14 18:48
---
## Level 1
### 함수 solution은 정수 n을 매개변수로 입력받습니다. 
### n의 각 자릿수를 큰것부터 작은 순으로 정렬한 새로운 정수를 리턴해주세요. 
### 예를들어 n이 118372 면  873211 을  리턴하면 됩니다.

**제한 조건**
> n은 1이상 8,000,000,000 이하인 자연수입니다.

**사용 언어 Python**

```python
def solution(n):
    answer = ''
    result = sorted(str(n),reverse = True)
    # n문자열 형변환 후 리스트 내림차순 정렬
    # result = ['8', '7', '3', '2', '1', '1']
    for i in range(len(result)):
        answer+=result[i]
    # for문 으로 list -> 문자열로 순서대로 넣음
    return int(answer)  # 문자열 answer int형변환 후 반환
```

### 차근차근 꾸준히 처음부터 하는 느낌으로 1일1코테 도전!!

---
layout: post
title: 자연수 뒤집어 배열만들기
categories: Python
author: Sowon Park
tags: [programers,codingTest,Python]
date: 2021-11-14 20:50
---
## Level 1
### 자연수 n을 뒤집어 각 자리 숫자를 원소로 가지는 배열 형태로 리턴해주세요. </br>예를들어 n이 12345이면 [5,4,3,2,1]을 리턴합니다.

**제한 조건**
> n은 10,000,000,000이하인 자연수입니다.

**입출력 예**
:------:
|n	    |return|
---::---
|12345	| [5,4,3,2,1]|
:------:

**사용언어 Python**  

```python
def list_revers(n):
    return list(map(int, reversed(str(n))))
    # n은 str 으로 변경후 revers 되고 map사용하여 int로 변경 list형변환
    # n = 12345 -> return 값 = [5,4,3,2,1]
```

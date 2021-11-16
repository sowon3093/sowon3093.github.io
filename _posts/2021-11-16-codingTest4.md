---
layout: post
title: 숫자 문자열과 영단어
categories: Python
author: Sowon Park
tags: [programers,codingTest,Python]
date: 2021-11-16 18:22
---
## Level 1
### 네오와 프로도가 숫자놀이를 하고 있습니다. <br/>네오가 프로도에게 숫자를 건넬 때 <br/>일부 자릿수를 영단어로 바꾼 카드를 건네주면 <br/>프로도는 원래 숫자를 찾는 게임입니다.

#### 다음은 숫자의 일부 자릿수를 영단어로 바꾸는 예시입니다.
> 1478 → "one4seveneight"
> 234567 → "23four5six7"
> 10203 → "1zerotwozero3"
이렇게 숫자의 일부 자릿수가 영단어로 바뀌어졌거나, <br/>혹은 바뀌지 않고 그대로인 문자열 s가 매개변수로 주어집니다. <br/>s가 의미하는 원래 숫자를 return 하도록 solution 함수를 완성해주세요.

**제한 조건**
> 1 ≤ s의 길이 ≤ 50
> s가 "zero" 또는 "0"으로 시작하는 경우는 주어지지 않습니다.
> return 값이 1 이상 2,000,000,000 이하의 정수가 되는 올바른 입력만 s로 주어집니다.


**사용언어 Python**  

```python
def solution(s):
    answer = 0
    key = {0:'zero',1:'one',2:'two',3:'three',4:'four',5:'five',
          6:'six',7:'seven',8:'eight',9:'nine'}

    for k,v in key.items():
        if v in s:
            s=s.replace(v,str(k))
    answer = s
    return int(answer)
```

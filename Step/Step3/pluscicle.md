특정 방법으로 더하기를 돌리고 횟수를 세기
=======

문제 및 코드
-----
[문제](https://www.acmicpc.net/problem/)




# 제출 코드

``` python

import math

a = int(input())
a1 = math.floor(a/10)
a0 = a-a1*10
i = 0

while True:
    b1= a0
    b0 = a1+a0-math.floor((a1+a0)/10)*10
    i = i+1
    if b1*10+b0 == a:
        break
    a1=b1
    a0=b0
print(i)


```


- - - - - 

설명
------

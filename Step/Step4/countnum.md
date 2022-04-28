각 자릿수에 써있는 숫자의 갯수를 세기
=======

문제 및 코드
-----
[문제](https://www.acmicpc.net/problem/2577)




# 제출 코드

``` python

import math

a=int(input())
b=int(input())
c=int(input())

n=a*b*c

ck = n
digit = 0
eachdata = []

while ck>=1:
    fin = ck-math.floor(ck/10)*10
    eachdata.insert(0, fin)
    ck=math.floor(ck/10)
    digit += 1

for i in range(10):
    print(eachdata.count(i))


```

## 참조
[각 자리에 써있는 수를 다루는 알고리즘](https://github.com/Sudkorea/IlovePython/blob/main/Step/tools/eachnumber.md)

- - - - - 

설명
------

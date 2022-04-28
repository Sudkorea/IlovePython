EOF로 임의의 숫자를 받다가 받을 것이 없으면 종료하기
=======

문제 및 코드
-----
[문제](https://www.acmicpc.net/problem/10951)




# 제출 코드

``` python

import sys

while True:
    try:
        a,b=map(int,sys.stdin.readline().split())
        print(a+b)
    except:
        break


```


- - - - - 

설명
------
try : except :를 연구해두자

A+B를 조금 더 print를 사용해서 표현하기
=======

문제 및 코드
-----
[문제](https://www.acmicpc.net/problem/11022)




# 제출 코드

``` python

import sys

case = int(input())

for i in range(case):
    a,b = map(int,sys.stdin.readline().split())
    c=i+1
    d=a+b
    print("Case #{}: {} + {} = {}".format(c, a, b, d))


```


- - - - - 

설명
------

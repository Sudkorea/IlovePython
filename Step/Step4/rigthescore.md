특정 방법으로 숫자를 조작하는 방법
=======

문제 및 코드
-----
[문제](https://www.acmicpc.net/problem/1546)




# 제출 코드

``` python

import sys

n=int(input())
tray=list(map(int,sys.stdin.readline().split()))
m=max(tray)
for j in range(n):
    tray[j] = (tray[j]/m)*100
print(sum(tray)/n)


```


- - - - - 

설명
------

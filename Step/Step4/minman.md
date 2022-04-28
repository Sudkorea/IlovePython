최솟값과 최댓값 구하기
=======

문제 및 코드
-----
[문제](https://www.acmicpc.net/problem/10818)




# 제출 코드

``` python

import sys

x=int(input())
data=list(map(int,sys.stdin.readline().split()))
data.sort()
print(data[0], data[x-1])


```


- - - - - 

설명
------
max, min 기능이 있는 것을 몰랐다.

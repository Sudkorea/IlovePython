리스트 중 작은 값만 나열하기
=======

문제 및 코드
-----
[문제](https://www.acmicpc.net/problem/10871)




# 제출 코드

``` python

import sys

n,x = input().split()
n=int(n)
x=int(x)
index=0
data = list(map(int,sys.stdin.readline().split()))

for i in range(n):
    if data[index]>=x:
        del data[index]
        index = index-1
    index = index + 1
print(' '.join(map(str, data)))


```


- - - - - 

설명
------
Index에 있는 값을 지우면 한칸씩 밀리는 것을 신경써주기

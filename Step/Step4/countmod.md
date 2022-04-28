나머지의 갯수를 세주자
=======

문제 및 코드
-----
[문제](https://www.acmicpc.net/problem/3052)




# 제출 코드

``` python

import sys

n=10
md=42
tray=[]
mod=[]

for i in range(n):
    num = int(sys.stdin.readline().rstrip())
    tray.append(num)
    
for j in tray:
    mod.append(j%md)
    
print(len(set(mod)))


```


- - - - - 

설명
------
중복된 것을 제거하는데는 

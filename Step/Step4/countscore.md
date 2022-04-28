가중치를 줘서 O의 갯수를 세기
=======

문제 및 코드
-----
[문제](https://www.acmicpc.net/problem/8958)




# 제출 코드

``` python

import sys

n = int(input())
tray=[]


for i in range(n):
    quiz=sys.stdin.readline().rstrip()
    tray.append(quiz)

for a in tray:
    point = 0
    mp = 0
    for i in range(len(a)):
        if a[i] == "O" and i == 0:
            point += 1
            mp += 1
            continue
        if a[i] == "O":
            if a[i-1] != a[i]:
                point += 1
            else:
                point = point + 1 + mp
            mp += 1
        else:
            mp = 0
    print(point)


```


- - - - - 

설명
------
점점 어려워지기 시작한다

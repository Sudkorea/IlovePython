평균을 구하고 퍼센트를 구하는데...
=======

문제 및 코드
-----
[문제](https://www.acmicpc.net/problem/)




# 제출 코드

``` python

import sys

n = int(input())
for i in range(n):
    count=0
    tray = list(map(int,sys.stdin.readline().split()))
    num=tray[0]
    avg=sum(tray[1:])/num
    for j in tray[1:]:
        if j>avg:
            count += 1
    print("{:.3f}%".format(round((count/num)*100,3)))


```


- - - - - 

설명
------
1. 문제 설명을 잘 읽고 하라는대로 하자
2. 정수형 데이터만 다루다 처음 실수형 데이터를 다루니 생긴 문제인데, 유효숫자를 챙겨주자 :,3f 등
3. 거의 2시간을 투자해서 맞췄다. 울뻔했다.

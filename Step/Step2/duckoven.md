오븐 시계 맞추기
=======

문제 및 코드
-----
[문제](https://www.acmicpc.net/problem/2525)




# 제출 코드

``` python

h,m=map(int, input().split())
c=int(input())
cm=c%60
if (m+cm)>=60:
    if (1+h+(c//60))>=24:
        print("{} {}".format(h+(c//60)-23,m+cm-60))
    else:
        print("{} {}".format(1+h+(c//60),m+cm-60))
else:
    if h+(c//60)>=24:
        print("{} {}".format(h+(c//60)-24,m+cm))
    else:
        print("{} {}".format(h+(c//60),m+cm))

```


- - - - - 

설명
------

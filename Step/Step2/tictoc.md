알람시계 맞추기
=======

문제 및 코드
-----
[문제](https://www.acmicpc.net/problem/2884)




# 제출 코드

``` python

h,m=map(int, input().split())
if m>=45:
    print("{} {}".format(h,m-45))
else:
    if h==0:
        print("{} {}".format(23,m+15))
    else:
        print("{} {}".format(h-1,m+15))

```


- - - - - 

설명
------

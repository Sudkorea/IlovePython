주사위 게임
=======

문제 및 코드
-----
[문제](https://www.acmicpc.net/problem/2480)




# 제출 코드

``` python

a,b,c=map(int, input().split())
S={a,b,c}
l=len(S)
if l==3:
    print(max(S)*100)
elif l==1:
    print(10000+max(S)*1000)
else:
    L=[a,b,c]
    if L.count(a) == 2:
        print(1000+a*100)
    else:
        print(1000+b*100)

```


- - - - - 

설명
------

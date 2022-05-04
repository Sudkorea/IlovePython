
=======

문제 및 코드
-----
[문제](https://www.acmicpc.net/problem/1193)




# 제출 코드

``` python
import numpy as np
import sys

n=int(input())
i=0

if n==1:
    print("1/1")
    sys.exit()

def pol2(x):
    return 2*(x**2)+3*x+1

while n>pol2(i):
    i += 1

move = np.array([-1,1])

if abs(n-pol2(i-1)-1)<abs(pol2(i)-n):
    x = 2*i
    count = pol2(i-1)+1
    cdn=np.array([x,1])
    while not count==n:
        cdn += move
        count += 1
else:
    x=2*i+1
    count = pol2(i)
    cdn=np.array([x,1])
    while not count==n:
        cdn += move
        count -= 1

print("{}/{}".format(cdn[1],cdn[0]))



```


- - - - - 

설명
------

아니 이보시오 numpy를 못쓰면 수학을 어떻게 


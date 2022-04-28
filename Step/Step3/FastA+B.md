입력이 많을때는 Input은 너무 느리다
=======

문제 및 코드
-----
[문제](https://www.acmicpc.net/problem/15552)




# 제출 코드

``` python

import sys

case = int(input())

for i in range(case):
    a,b = map(int,sys.stdin.readline().split())
    print(a+b)

```


- - - - - 

설명
------
이럴때 사용하는 것이 sys.stdin.readline()

아직 완벽히 이해하진 못했다.

변수가 많을 경우 뒤에 split(), 문자열을 받는데 개행문자는 제외하고 싶을 때는 rstrip()을 

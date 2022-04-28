모듈러 연산의 분배법칙에 대해
=======

문제 및 코드
-----
[문제](https://www.acmicpc.net/problem/10430)




# 제출 코드

A,B,C=map(int, input().split())

print((A+B)%C)

print(((A%C)+(B%C))%C)

print((A*B)%C)

print(((A%C)*(B%C))%C)

- - - - - 

설명
------
분배법칙이 성립한다는 것을 알 수 있다.

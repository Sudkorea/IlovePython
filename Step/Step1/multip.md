곱셈식 중 일부를 채우기
=======

문제 및 코드
-----
[문제](https://www.acmicpc.net/problem/2588)




# 제출 코드

A=int(input())

B=int(input())

E=B

while B>0:

    C=B%10
    
    B=B//10
    
    print(A*C)
    
print(A*E)



- - - - - 

설명
------
아직 While을 쓸 때가 아닌거같긴 한데

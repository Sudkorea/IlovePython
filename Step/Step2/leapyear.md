강한친구 대한육군
=======

문제 및 코드
-----
[문제](https://www.acmicpc.net/problem/2753)




# 제출 코드

n=int(input())

if (n%4 == 0):

    if (n%100 == 0):
    
        if (n%400 == 0):
        
            print('1')
            
        else:
        
            print('0')
            
    else:
    
        print('1')
        
else:

    print('0')




- - - - - 

설명
------

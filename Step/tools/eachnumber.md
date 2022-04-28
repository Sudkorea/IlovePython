자연수가 주어지면 각 자리수를 떼서 저장하기
=========

코드
------

```` python
import math

n=int(input())

if abs(math.floor(n)) != n:
    quit()

ck = n
digit = 0
eachdata = []

while ck>=1:
    fin = ck-math.floor(ck/10)*10
    eachdata.insert(0, fin)
    ck=math.floor(ck/10)
    digit += 1
    
   
```


- - - - - - -


#설명
임의의 자연수가 들어오면, 각 자리수를 떼어 리스트에 저장하는 알고리즘을 만들어보았다.

문자열로 배열한 뒤 떼주는 방법을 생각 못한 수학과는, floor 함수를 통해 한 자리씩 떼주는 방법을 사용하였다.

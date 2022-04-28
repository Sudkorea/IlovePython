배열의 최댓값과 위치를 구하기
=======

문제 및 코드
-----
[문제](https://www.acmicpc.net/problem/2562)




# 제출 코드

``` python

data = []
n = 9
for i in range(n):
    data.append(int(input()))


m = max(data)
n = data.index(m)+1
print("{}\n{}".format(m,n))


```


- - - - - 

설명
------
세로형의 데이터를 가로로 나열하여 최댓값을 구하고 검색기능으로 위치를 찾기

행렬을 이용해볼까 했으나 나중에 해보기로

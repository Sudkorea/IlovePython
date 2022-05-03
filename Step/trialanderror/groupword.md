
=======

문제 및 코드
-----
[문제](https://www.acmicpc.net/problem/1316)




# 제출하려다가막힌코드

``` python
n = input()
n = list(n)
nset = set(n)
count = nset

for ele in nset:
    globals()["pt_{}".format(ele)] = [i for i, alp in enumerate(n) if alp == ele]
    
tray = [0 for i in range(len(nset))]

for ele in nset:
    if range(len(globals()["pt_{}".format(ele)])) == 1:
        continue
    elif range(len(globals()["pt_{}".format(ele)])) == 2:
        if abs(globals()["pt_{}".format(ele)][0]-globals()["pt_{}".format(ele)][1]) != 1:
            count.discard(ele) 
    else:
        for j in range(len(globals()["pt_{}".format(ele)])-2):
            if abs(globals()["pt_{}".format(ele)][j]-globals()["pt_{}".format(ele)][j+1]) != 1:
                count.discard(ele) 
                continue
        
print(len(count))



```


- - - - - 

설명
------
한개의 문장을 받았을 때 그 문자가 얼마나 쓰였나를 써주는 알고리즘(2차원 배열에 대해 아는 것이 없어서 중단됨)

한 문장 속에서 개별적인 단어가 그룹 단어인줄 착각하고 만든, 그룹 단어만 남기기 위해 집합을 만들고 그 중 필요한 것만 남기는 알고리즘

열심히 썼는데 좀 다르게 접근할 필요가 있어서, 지우기 전에 남겨둠.

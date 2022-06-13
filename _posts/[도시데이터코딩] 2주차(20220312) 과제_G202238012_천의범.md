## 1. 튜플 문제

### 요구 사항에 맞춰 슬라이싱하기

![image.png](data:image/png;base64,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)


```python
#교통공학과 천의범
print('index 0부터 3까지:', numbers[0:4]) # "" 위치 채우기
print('index 2부터 4까지:', numbers[2:5]) # "" 위치 채우기
print('index 3부터 끝까지:', numbers[3:]) # "" 위치 채우기
print('index 2부터 뒤에서 -2까지:', numbers[2:-2]) # "" 위치 채우기
print('index 0부터 끝까지, 3단계:', numbers[0::3]) # "" 위치 채우기
import numpy as np
print('최소값:', np.min(numbers)) # "" 위치 채우기
print('최대값:', np.max(numbers)) # "" 위치 채우기

print('최소값 index 위치:', numbers.index(np.min(numbers))) # "" 위치 채우기
print('최대값 index 위치:', numbers.index(np.max(numbers))) # "" 위치 채우기

print('최소값 index 위치:', np.argmin(numbers)) # "" 위치 채우기
print('최대값 index 위치:', np.argmax(numbers)) # "" 위치 채우기
```

    index 0부터 3까지: [2, 3, 5, 7]
    index 2부터 4까지: [5, 7, 9]
    index 3부터 끝까지: [7, 9, 11, 13]
    index 2부터 뒤에서 -2까지: [5, 7, 9]
    index 0부터 끝까지, 3단계: [2, 7, 13]
    최소값: 2
    최대값: 13
    최소값 index 위치: 0
    최대값 index 위치: 6
    최소값 index 위치: 0
    최대값 index 위치: 6
    

## 2. 리스트 문제

### 7개의 숫자 중 서로 다른 숫자 2개를 나열하는 모든 경우의 수를 출력하는 프로그램 만들기

![image.png](data:image/png;base64,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)


```python
#교통공학과 천의범
numbers = [2,3,5,7,9,11,13]
result = []

"""아래 내용으로 소스 채우기"""
for i in range(len(numbers)):
    for j in range(len(numbers)):
        if numbers[i]==numbers[j]:
            continue
        result.append([numbers[i],numbers[j]])
    
    
print('result:', result)
print('result length:', len(result)) # 경우의 수 출력
```

    result: [[2, 3], [2, 5], [2, 7], [2, 9], [2, 11], [2, 13], [3, 2], [3, 5], [3, 7], [3, 9], [3, 11], [3, 13], [5, 2], [5, 3], [5, 7], [5, 9], [5, 11], [5, 13], [7, 2], [7, 3], [7, 5], [7, 9], [7, 11], [7, 13], [9, 2], [9, 3], [9, 5], [9, 7], [9, 11], [9, 13], [11, 2], [11, 3], [11, 5], [11, 7], [11, 9], [11, 13], [13, 2], [13, 3], [13, 5], [13, 7], [13, 9], [13, 11]]
    result length: 42
    


```python
#연습
numbers = [2,3,5,7,9,11,13]

for i in range(len(numbers)):
    for j in range(len(numbers)):
        result=[]
        if numbers[i]==numbers[j]:
            continue
        print([numbers[i],numbers[j]],end=",")
    
```

    [2, 3],[2, 5],[2, 7],[2, 9],[2, 11],[2, 13],[3, 2],[3, 5],[3, 7],[3, 9],[3, 11],[3, 13],[5, 2],[5, 3],[5, 7],[5, 9],[5, 11],[5, 13],[7, 2],[7, 3],[7, 5],[7, 9],[7, 11],[7, 13],[9, 2],[9, 3],[9, 5],[9, 7],[9, 11],[9, 13],[11, 2],[11, 3],[11, 5],[11, 7],[11, 9],[11, 13],[13, 2],[13, 3],[13, 5],[13, 7],[13, 9],[13, 11],

## 3. 딕셔너리 문제

### 딕셔너리를 이용해 5명의 회원을 가입 받고 전체 회원 정보를 출력하는 프로그램 만들기
#### 1) 회원 이메일 입력 받고, 비밀번호 입력 받기
#### 2) 동일한 이메일이 입력으로 들어오게 되면, 아래와 같이 공지 후 다시 입력 받기

![image.png](data:image/png;base64,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)


```python
#교통공학과 천의범
# 딕셔너리를 이용해 5명의 회원을 가입 받고 전체 회원 정보를 출력하는 프로그램 만들기
members = {} # 회원을 담을 dict
n = 1

while n < 6:
    mail = input('메일 입력: ')
    pw = input('비번 입력: ')
    
    if mail in members:
        print("이미 사용중인 메일 계정입니다")
        continue
    else:
        members[mail]=pw
        n+=1

# 5번이 다 돌아가고 정보가 다 저장이 되고 출력하기
for key in members.keys():
    print(f'{key} : {members[key]}') # members의 key와 해당 key값에 해당하는 value 출력
```

    메일 입력: haha@gmail.com
    비번 입력: haha
    메일 입력: a@a.a
    비번 입력: a
    메일 입력: b@b.b
    비번 입력: b
    메일 입력: a@a.a
    비번 입력: a
    이미 사용중인 메일 계정입니다
    메일 입력: b@b.b
    비번 입력: b
    이미 사용중인 메일 계정입니다
    메일 입력: c@c.c
    비번 입력: d@d.d
    메일 입력: e@e.e
    비번 입력: e@e.e
    haha@gmail.com : haha
    a@a.a : a
    b@b.b : b
    c@c.c : d@d.d
    e@e.e : e@e.e
    

## 4. 함수 문제

### print_arithmetic_operation 함수에 숫자 2개를 넣었을 때 
### 사칙연산 결과를 아래와 같이 출력해주는 함수 구현하기

![image.png](data:image/png;base64,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)


```python
#교통공학과 천의범
# 함수코드 작성하기

def print_arithmetic_operation(x,y):
    print(x,"+",y,"=", x+y)
    print(x,"-",y,"=", x-y)
    print(x,"*",y,"=", x*y)
    print(x,"/",y,"=", x/y)
          
# 함수 실행하기
print_arithmetic_operation(3, 4)

# 함수코드 작성하기 (문제와 같은 형태)
print("")
def print_arithmetic_operation(x,y):
    print(x,"+",y,"=", x+y)
    print(x,"-",y,"=", x+y)
    print(x,"*",y,"=", x+y)
    print(x,"/",y,"=", x+y)
          
# 함수 실행하기
print_arithmetic_operation(3, 4)
```

    3 + 4 = 7
    3 - 4 = -1
    3 * 4 = 12
    3 / 4 = 0.75
    
    3 + 4 = 7
    3 - 4 = 7
    3 * 4 = 7
    3 / 4 = 7
    

## 5. 파일 입출력 문제

### 1) 아래 리스트에 있는 각 숫자들을 라인 단위로 파일에 입력하기 ( 파일명은 strings.txt )
### 2) numbers.txt 파일 읽어서 다시 strings와 동일한 strings2 만들기

![image.png](data:image/png;base64,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)

![image.png](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAJ8AAAA9CAYAAACzz7sFAAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsMAAA7DAcdvqGQAAAKhSURBVHhe7dsLbqswEIVh2oVkHVlDtpGNZCPZRrZ3q1Ez0tTXBvOwD4T/k1ARY8CWTw3p4+tyufwbAIHv91egO8IHGcIHGcIHmerwPR6P915ZTZs9e71e77327F5xO6Oq8B0peEeYSOvj7Xb7s50xgJuF7xNYCNDPJu98Fs6eAfVHlW/O99PjrrYeedvSOSbWYhs/HuuGkP863AcOm8T4uLLNJ9Yn1Y/nxPNreXvbYohMvF6sxeO5euRtz2Z1+HqvejlzJm7LSU5DM3XtXP2swTOHW/lsomzCSqvIXtT088zBM6vCp1r1bMKOEMKxfp49eGazx66HsGcY4+QqpPcu9SPtJ8H7tcnK1zN8qqCVeKjSQO2tn3t06He+3KTHemt+D7tn7IOZ6mdas+1s+Hu+ldLQpCFEGeGDzOEeu/gchA8yhA8yhA8yhA8yhA8yhA8yhA8yhA8yhA8yhA8yhA8yhA8yX9frlb9qgQQrH2QIH2QIH2QIH2QIH2QIH2QIH2QIH2Qmf8j8fD7fe8Nwv9/fe8BfS3JStfLZxXIXjDfMsfpUmzm2vJbLXbPFfdynjqGUkTHNHrvWwSUdwnnwzgeZqne+uatXuiyn53s9d92xWi8+5lJf4vhytbFze1k6hng8qh2H37dGk/CZ0nnxeNpmrNaT3dvk+jLWZ5Oeq7JmDKmpejSnbdfHbtox27djZqymUOpLPF5S06aHNWNw6bxsiXe+BWxCfDuqmjFYreU3EuGbySfEtyOqGUPr4BnCh//0CJ7pGj4bkA3MxUGO1WrEc7dQ05eW99zCkjGU2rXQfeXzkOUGOVbrrdSX3HHb36OlY/Ba3Fr4iN/tWh/32rdaRx/Dkpzw32uQ4QMHZAgfZAgfZAgfZAgfZAgfZAgfRIbhB2SnFQokjmywAAAAAElFTkSuQmCC)


```python
#교통공학과 천의범
strings = ["foo", "bar", "baz"]

# 파일에 내용 입력하기 strings.txt
with open('strings.txt', 'w') as ub:
    for name in strings:
        ub.write(name+'\n')
ub.close()
```


```python
#실제로 저장된 파일 형태
!pip install IPython
from IPython.display import Image
Image("image.JPG")
```

    Requirement already satisfied: IPython in e:\arcgispro\bin\python\envs\arcgispro-py3\lib\site-packages (7.18.1)
    Requirement already satisfied: traitlets>=4.2 in e:\arcgispro\bin\python\envs\arcgispro-py3\lib\site-packages (from IPython) (4.3.3)
    Requirement already satisfied: setuptools>=18.5 in e:\arcgispro\bin\python\envs\arcgispro-py3\lib\site-packages (from IPython) (49.6.0.post20200814)
    Requirement already satisfied: pickleshare in e:\arcgispro\bin\python\envs\arcgispro-py3\lib\site-packages (from IPython) (0.7.5)
    Requirement already satisfied: prompt-toolkit!=3.0.0,!=3.0.1,<3.1.0,>=2.0.0 in e:\arcgispro\bin\python\envs\arcgispro-py3\lib\site-packages (from IPython) (3.0.5)
    Requirement already satisfied: decorator in e:\arcgispro\bin\python\envs\arcgispro-py3\lib\site-packages (from IPython) (4.4.2)
    Requirement already satisfied: pygments in e:\arcgispro\bin\python\envs\arcgispro-py3\lib\site-packages (from IPython) (2.7.0)
    Requirement already satisfied: colorama; sys_platform == "win32" in e:\arcgispro\bin\python\envs\arcgispro-py3\lib\site-packages (from IPython) (0.4.3)
    Requirement already satisfied: jedi>=0.10 in e:\arcgispro\bin\python\envs\arcgispro-py3\lib\site-packages (from IPython) (0.17.2)
    Requirement already satisfied: backcall in e:\arcgispro\bin\python\envs\arcgispro-py3\lib\site-packages (from IPython) (0.2.0)
    Requirement already satisfied: six in e:\arcgispro\bin\python\envs\arcgispro-py3\lib\site-packages (from traitlets>=4.2->IPython) (1.15.0)
    Requirement already satisfied: ipython-genutils in e:\arcgispro\bin\python\envs\arcgispro-py3\lib\site-packages (from traitlets>=4.2->IPython) (0.2.0)
    Requirement already satisfied: wcwidth in e:\arcgispro\bin\python\envs\arcgispro-py3\lib\site-packages (from prompt-toolkit!=3.0.0,!=3.0.1,<3.1.0,>=2.0.0->IPython) (0.2.5)
    Requirement already satisfied: parso<0.8.0,>=0.7.0 in e:\arcgispro\bin\python\envs\arcgispro-py3\lib\site-packages (from jedi>=0.10->IPython) (0.7.0)
    




    
![jpeg](output_22_1.jpg)
    




```python
strings
```




    ['foo', 'bar', 'baz']




```python
# 파일에서 내용 출력하기
f = open("strings.txt","r")
lines = f.readlines()

# strings2 출력하기
strings2 = list(map(lambda x: x.strip(), lines))
print(strings2)
```

    ['foo', 'bar', 'baz']
    

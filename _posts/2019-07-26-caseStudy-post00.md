---
title:  "중첩 반복문 - 행열 다루기 - 대체하기"
published: true
permalink: m3_1_forloopIfElseTest.html
summary: "This is forloopIfElseTest example for post.(m3_1_forloopIfElseTest)"
tags: [posts, news, getting_started, python, caseStudy]
sidebar: news_sidebar
keywords: python, program, caseStudy, Dictionary
---

## Execution Result

## caseStudy - 중첩 반복문 - 행열 다루기 - 대체하기

요구사항: 배열 값이 6이상이면 5로 나눈 나머지 값으로 대체한다.

### 1.inputData, iniArr, arrSize변수 선언과 초기화
```
  inputData = [                 
      [1, 2, 3, 5, 4, 3],  
      [2, 3, 5, 3, 2, 4],  
      [3, 5, 3, 2, 4, 6],  
      [4, 3, 4, 5, 6, 3],  
      [5, 1, 5, 8, 5, 2],  
      [6, 5, 8, 5, 4, 1]   
  ]  
  iniArr = []  
  arrSize = len(inputData)  
  iniArr = [[0 for row in range(arrSize)] for col in range(arrSize)]  
```
### 2.문자열 함수와 반복 실행하는 반복문

요구사항: 배열 값이 6이상이면 5로 나눈 나머지 값으로 대체한다.

```
  for i in range(arrSize):             
      for j in range(arrSize):  
          num = inputData[i][j]  
          if num >= 6:  
              iniArr[i][j] = num % 5  
          else:  
              iniArr[i][j] = num  
```
### 3.결과값 출력문
```
  for i in range(arrSize):             
      for j in range(arrSize):  
          num = inputData[i][j]  
          if num >= 6:  
              iniArr[i][j] = num % 5  
          else:  
              iniArr[i][j] = num  
          print(iniArr[i][j], end="	")  
      print("")  
```
### 4.결과값
```
1	2	3	5	4	3
2	3	5	3	2	4
3	5	3	2	4	1
4	3	4	5	1	3
5	1	5	3	5	2
1	5	3	5	4	1
```
### 5.프로그램 종료
```
  print("Program End")
  Program End
```
## Program Source

```
print('caseStudy - 중첩 반복문 - 행열 다루기 - 대체하기')
print('m3_1_forloopIfElseTest.py\n')

print("1.inputData, iniArr, arrSize변수 선언과 초기화\n")
print('  inputData = [                 ')
print('      [1, 2, 3, 5, 4, 3],  ')
print('      [2, 3, 5, 3, 2, 4],  ')
print('      [3, 5, 3, 2, 4, 6],  ')
print('      [4, 3, 4, 5, 6, 3],  ')
print('      [5, 1, 5, 8, 5, 2],  ')
print('      [6, 5, 8, 5, 4, 1]   ')
print('  ]  ')
print('  iniArr = []  ')
print('  arrSize = len(inputData)  ')
print('  iniArr = [[0 for row in range(arrSize)] for col in range(arrSize)]  ')
inputData = [
    [1, 2, 3, 5, 4, 3],
    [2, 3, 5, 3, 2, 4],
    [3, 5, 3, 2, 4, 6],
    [4, 3, 4, 5, 6, 3],
    [5, 1, 5, 8, 5, 2],
    [6, 5, 8, 5, 4, 1]
]
iniArr = []
arrSize = len(inputData)
iniArr = [[0 for row in range(arrSize)] for col in range(arrSize)]
print()
print("2.문자열 함수와 반복 실행하는 반복문\n")
print('  for i in range(arrSize):             ')
print('      for j in range(arrSize):  ')
print('          num = inputData[i][j]  ')
print('          if num >= 6:  ')
print('              iniArr[i][j] = num % 5  ')
print('          else:  ')
print('              iniArr[i][j] = num  ')
print()
print("3.결과값 출력문\n")
print('  for i in range(arrSize):             ')
print('      for j in range(arrSize):  ')
print('          num = inputData[i][j]  ')
print('          if num >= 6:  ')
print('              iniArr[i][j] = num % 5  ')
print('          else:  ')
print('              iniArr[i][j] = num  ')
print('          print(iniArr[i][j], end="\t")  ')
print('      print("")  ')
print()
print("4.결과값\n")
for i in range(arrSize):
    for j in range(arrSize):
        num = inputData[i][j]
        # iniArr[i][j] = num
        if num >= 6:
            iniArr[i][j] = num % 5
        else:
            iniArr[i][j] = num
        # print(num, end="\t" )
        # print(iniArr[i][j], end="\t" )
        print(iniArr[i][j], end="\t")
    print("")
print()
print('5.프로그램 종료\n')
print('  print("Program End")\n')
print("  Program End")
```

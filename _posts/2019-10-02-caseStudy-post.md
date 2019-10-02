title:  'SECTION002_20 알고리즘-수열2: 1에서 100까지 부호 교차의 합계-방안2'
published: true
permalink: SECTION002_20_forloopTest_003.html
summary: "This is forloopTest example for post.(forloopTest)"
tags: [posts, news, getting_started, python, case_study]
sidebar: posts_sidebar
keywords: python, program, caseStudy, Dictionary
---

## Execution Result

## SECTION002_20 알고리즘-수열2: 1에서 100까지 부호 교차의 합계-방안2

## 1. i, sum 변수 선언과 초기화
```
   i, sum = 0, 0  #j 대신에 이해를 위해 sum 변수 사용
```
## 2. 반복문 내 조건문을 실행하는 반복 조건문
```
   for i in range(1, 101, 2) : # 2개를 하나의 단위로
       sum = sum + i
       i = i + 1    
       sum = sum - i
   print(" 결과값->")
   print(" sum = ", sum)
```
## 3. 결과값 출력문
```
   print("   sum = ", sum)
```
## 4. 결과값 출력
```
   sum =  -50
```
## 5. 프로그램 종료문
```
   print("Program End")
```
## 6. 프로그램 종료
```
   Program End
```

## Program Source

```
print("SECTION002_20 알고리즘-수열2: 1에서 100까지 부호 교차의 합계-방안2")
print()
print("1. i, sum 변수 선언과 초기화 ")
print("   i, sum = 0, 0  #j 대신에 이해를 위해 sum 변수 사용")
i, sum = 0, 0
print()
print("2. 반복문 내 조건문을 실행하는 반복 조건문 ")
print("   for i in range(1, 101, 2) : # 2개를 하나의 단위로")
print("       sum = sum + i")
print("       i = i + 1    ")
print("       sum = sum - i")
print('   print(" 결과값->")')
print('   print(" sum = ", sum)')
print()
for i in range(1, 101, 2) :    # 2개를 하나의 단위로 첫번째 항
    # print(i)                 # 검증용
    sum = sum + i
    # print("   sum = ", sum)  # 검증용
    i = i + 1                  # 두번째 항을 만들어준다.
    # print(i)                 # 검증용
    sum = sum - i
    # print("   sum = ", sum)  # 검증용
print("3. 결과값 출력문")
print('   print("   sum = ", sum)')
print()
print("4. 결과값 출력")
print("   sum = ", sum)
print()
print('5. 프로그램 종료문')
print('   print("Program End")')
print()
print('6. 프로그램 종료')
print("   Program End")
```

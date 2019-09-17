---
title:  'SECTION002_10 알고리즘-수열2: 1에서 100까지 부호 교차의 합계-방안1'
published: true
permalink: forloopIfelseTest_Section002_10.html
summary: "This is forloopIfelseTest example for post.(forloopIfelseTest)"
tags: [posts, section, python]
sidebar: posts_sidebar
keywords: python, program, section
---

## Execution Result

**주어진 i, sum, sw 변수를 이용해 1에서 100까지 부호 교차의 합계를 구한다.
  {1, -2, 3, -4, 5,..99, -100}**

## SECTION002_10 알고리즘-수열2: 1에서 100까지 부호 교차의 합계-방안1

### 1. i, sum, sw 변수 선언과 초기화:
```
   i, sum, sw = 0, 0, 0  #j 대신에 이해를 위해 sum 변수 사용
```
### 2. 반복문 내 조건문을 실행하는 반복 조건문
```
   for i in range(1, 101, 1) :
       if sw == 0 :
          sum = sum + i
          sw = 1
        else:
          sum = sum - i
          sw = 0
```
### 3. 결과값 출력문
```
   print("   sum = ", sum)
```
### 4. 결과값 출력
```
   sum =  -50
```
### 5. 프로그램 종료문
```
   print("Program End")
```
### 6. 프로그램 종료
```
   Program End
```

## Program Source

```
print("SECTION002_10 알고리즘-수열2: 1에서 100까지 부호 교차의 합계-방안1")
print()
print("1. i, sum, sw 변수 선언과 초기화: ")
print("   i, sum, sw = 0, 0, 0  #j 대신에 이해를 위해 sum 변수 사용")
i, sum, sw = 0, 0, 0
print()
print("2. 반복문 내 조건문을 실행하는 반복 조건문")
print("   for i in range(1, 101, 1) :")
print("       if sw == 0 :")
print("          sum = sum + i")
print("          sw = 1")
print("        else:")
print("          sum = sum - i")
print("          sw = 0")
print()
for i in range(1, 101, 1) :
    #print("i = ", i)
    if sw == 0 :
        sum = sum + i
        #print("   sum = ", sum)              # 검증용
        sw = 1                                # 최초 0에서 1로 변경
    else:
        sum = sum - i
        #print("   sum = ", sum)              # 검증용
        sw = 0                                # 1에서 0로 변경
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

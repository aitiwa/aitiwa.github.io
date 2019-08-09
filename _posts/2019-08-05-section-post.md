---
title:  '알고리즘-1에서 100까지 합계'
published: true
permalink: forloopTest_003_Section001.html
summary: "This is forloopTest example for post.(forloopTest)"
tags: [posts, section, python]
sidebar: posts_sidebar
keywords: python, program, section
---

## Execution Result

**주어진 i, sum 변수를 이용해 1에서 100까지 합계를 구한다.**

## Section001 알고리즘-1에서 100까지 합계

### 1. i, sum 변수 선언과 초기화:
```
   i, sum = 0, 0
```
### 2. 반복 계산하는 반복문:
```
   for i in range(1, 101, 1) :
       sum = sum + i    # sum += i
```
### 3. 결과값 출력문
```
   print("   sum = ", sum)
```
### 4. 결과값 출력
```
   sum =  5050
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
print("Section001 알고리즘-1에서 100까지 합계\n")
print("forloopTest_003")
print()
print("1. i, sum 변수 선언과 초기화: ")
print("   i, sum = 0, 0")
i, sum = 0, 0      #j 대신에 sum 변수 사용
print()
print("2. 반복 계산하는 반복문: ")
print("   for i in range(1, 101, 1) :")
print("       sum = sum + i")
print('   print(" 결과값->")')
print('   print(" sum = ", sum')
print()
for i in range(1, 101, 1) :
    sum = sum + i
    # print("{}, {}".format(i,sum))   # 검증
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

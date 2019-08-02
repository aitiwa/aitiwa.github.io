---
title:  '반복문-문자열 다루기 - "HelloKOREA" 반복회수 계산 사례'
published: true
permalink: forloopTest.html
summary: "This is forloopTest example for post.(forloopTest)"
tags: [posts, news, getting_started, python, case_study]
sidebar: posts_sidebar
keywords: python, program, caseStudy, Dictionary
---

## Execution Result

## 반복문-문자열 다루기 - "HelloKOREA" 반복회수 계산 사례

### 1. str1, list1, result,dic1_count 변수 선언과 초기화
```
   str1 = "HelloKOREAA"
   list1 = list(str1)   
   result1 = ""         
   dic1_count = {}      
```
### 2. Dictionary와 반복 실행하는 반복문
```
   for i in list1:                       
        if i not in dic1_count.keys():  
           dic1_count[i] = 1  
        else:  
           dic1_count[i] += 1  
```
### 3. 결과값 출력문
```
   print("   dic1_count = ", dic1_count)
```
### 4. 결과값
```
   dic1_count =  {'H': 1, 'e': 1, 'l': 2, 'o': 1, 'K': 1, 'O': 1, 'R': 1, 'E': 1, 'A': 2}
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
print('caseStudy - 반복문-문자열 다루기 - "HelloKOREA" 반복회수 계산 사례')
print('forloopTest')
print()
print("1. str1, list1, result,dic1_count 변수 선언과 초기화 ")
print('   str1 = "HelloKOREAA" ')
print('   list1 = list(str1)   ')
print('   result1 = ""         ')
print("   dic1_count = {}      ")
str1 = "HelloKOREAA"
list1 = list(str1)
result1 = ""
dic1_count = {}
print()
print("2. Dictionary와 반복 실행하는 반복문 ")
print('   for i in list1:                       ')
print('        if i not in dic1_count.keys():  ')
print('           dic1_count[i] = 1  ')
print('        else:  ')
print('           dic1_count[i] += 1  ')
for i in list1:
     if i not in dic1_count.keys():
        dic1_count[i] = 1
     else:
        dic1_count[i] += 1
print()
print("3. 결과값 출력문")
print('   print("   dic1_count = ", dic1_count) ')
print()
print("4. 결과값")
print("   dic1_count = ", dic1_count)
print()
print('5. 프로그램 종료문')
print('   print("Program End")')
print()
print('6. 프로그램 종료')
print("   Program End")
```

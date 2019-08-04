---
title:  '반복문-문자열 다루기 - "HelloKOREA" 반복회수 계산 사례3'
published: true
permalink: forloopIfElseTest_003.html
summary: "This is forloopIfElseTest example for post.(forloopIfElseTest)"
tags: [posts, news, python, case_study]
sidebar: posts_sidebar
keywords: python, program, caseStudy, Dictionary
---

## Execution Result

**주어진 문자열을 리스트로 바꾸고 Dictionary의 세트 정보를 이용해
반복되는 회수를 Count하고 해당 세트 정보를 출력한다.**

## 반복문-문자열 다루기 - "HelloKOREA" 반복회수 계산 사례

### 1. str1, list1, dic1_count 변수 선언과 초기화
```
   str1 = "HelloKOREAA"
   list1 = list(str1)          
   dic1_count = {}      
```
### 2. Dictionary변수와 반복문을 이용한 반복 회수를 계산하는 반복문
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
   print('   print("   dic1_count.items() = ", dic1_count.items()) ')
   print('   print("   dic1_count.keys() = ", dic1_count.keys()) ')
   print('   print("   dic1_count.values() = ", dic1_count.values()) ')
```
### 4. 결과값
```
   dic1_count =  {'H': 1, 'e': 1, 'l': 2, 'o': 1, 'K': 1, 'O': 1, 'R': 1, 'E': 1, 'A': 2}
   dic1_count.items() =  dict_items([('H', 1), ('e', 1), ('l', 2), ('o', 1), ('K', 1), ('O', 1), ('R', 1), ('E', 1), ('A', 2)])
   dic1_count.keys() =  dict_keys(['H', 'e', 'l', 'o', 'K', 'O', 'R', 'E', 'A'])
   dic1_count.values() =  dict_values([1, 1, 2, 1, 1, 1, 1, 1, 2])
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
print('caseStudy - 반복문-문자열 다루기 - "HelloKOREA" 반복회수 계산 사례3')
print('forloopIfElseTest')
print()
print("1. str1, list1, dic1_count 변수 선언과 초기화 ")
print('   str1 = "HelloKOREAA" ')
print('   list1 = list(str1)   ')
print("   dic1_count = {}      ")
str1 = "HelloKOREAA"
list1 = list(str1)
dic1_count = {}
print()
print("2. Dictionary와 반복 반복 회수를 계산하는 반복문 ")
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
print('   print("   dic1_count.items() = ", dic1_count.items()) ')
print('   print("   dic1_count.keys() = ", dic1_count.keys()) ')
print('   print("   dic1_count.values() = ", dic1_count.values()) ')
print()
print("4. 결과값")
print("   dic1_count = ", dic1_count)
print("   dic1_count.items() = ", dic1_count.items())
print("   dic1_count.keys() = ", dic1_count.keys())
print("   dic1_count.values() = ", dic1_count.values())
print()
print('5. 프로그램 종료문')
print('   print("Program End")')
print()
print('6. 프로그램 종료')
print("   Program End")
```

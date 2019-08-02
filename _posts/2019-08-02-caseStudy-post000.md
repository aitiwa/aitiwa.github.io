---
title:  '반복문-문자열 다루기 - "HelloKOREA" 반복회수 계산 조건값 사례4'
published: true
permalink: forloopIfElseTest_004.html
summary: "This is forloopIfElseTest example for post.(forloopIfElseTest)"
tags: [posts, news, getting_started, python, case_study]
sidebar: posts_sidebar
keywords: python, program, caseStudy, Dictionary
---

## Execution Result

**주어진 문자열을 리스트로 바꾸고 Dictionary의 세트 정보를 이용해
반복되는 회수를 Count하고 2개 이상인 세트 정보를 출력한다.**

## 반복문-문자열 다루기 - "HelloKOREA" 반복회수 계산 조건값 사례4

### 1.1 str1, size, list1, dic1_count 변수 선언과 초기화
```
    str1 = "HelloKOREAA"
    size = len(str1)
    list1 = list(str1)
    dic1_count = {}
```
### 2.1 문자열 함수와 반복 회수 계산하는 반복문
```
    for i in list1:                       
         if i not in dic1_count.keys():  
            dic1_count[i] = 1  
         else:  
            dic1_count[i] += 1  
```
### 3.1 결과값 출력문
```
    print("   dic1_count = ", dic1_count)
```
### 4.1 결과값
```
    dic1_count =  {'H': 1, 'e': 1, 'l': 2, 'o': 1, 'K': 1, 'O': 1, 'R': 1, 'E': 1, 'A': 2}
```
### 1.2 cnt, searchword 변수 선언과 초기화  
```
    cnt = 0         
    searchword = ""
```
### 2.2 최대값 계산하는 반복문
```
    for word, cnt in dic1_count.items() :   
        if cnt > 1 :  
            searchWord = word  
```
### 3.2 결과값 출력문
```
            print("    " + searchWord + "->" + str(cnt))  
```
### 4.2 결과값
```
    l->2
    A->2
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
print('caseStudy - 반복문-문자열 다루기 - "HelloKOREA" 반복회수 계산 최대값 사례4')
print('forloopIfElseTest_004')
print()
print("1.1 str1, size, list1, dic1_count 변수 선언과 초기화  ")
print('    str1 = "HelloKOREAA" ')
print('    size = len(str1) ')
print('    list1 = list(str1) ')
print("    dic1_count = {}")
str1 = "HelloKOREAA"
size = len(str1)
list1 = list(str1)
dic1_count = {}
print()
print("2.1 문자열 함수와 반복 회수 계산하는 반복문 ")
print('    for i in list1:                       ')
print('         if i not in dic1_count.keys():  ')
print('            dic1_count[i] = 1  ')
print('         else:  ')
print('            dic1_count[i] += 1  ')
for i in list1:
     if i not in dic1_count.keys():
        dic1_count[i] = 1
     else:
        dic1_count[i] += 1
print()
print("3.1 결과값 출력문")
print('    print("   dic1_count = ", dic1_count) ')
print()
print("4.1 결과값")
print("    dic1_count = ", dic1_count)
print()
print("1.2 cnt, searchword 변수 선언과 초기화  ")
print('    cnt = 0         ')
print('    searchword = "" ')
cnt = 0
searchword = ""
print()
print("2.2 최대값 계산하는 반복문 ")
print('    for word, cnt in dic1_count.items() :   ')
print('        if cnt > 1 :  ')
print('            searchWord = word  ')
for word, cnt in dic1_count.items() :
    if cnt > 1 :
        searchWord = word
print()
print("3.2 결과값 출력문")
print('            print("    " + searchWord + "->" + str(cnt))  ')
print()
print("4.2 결과값")
cnt = 0
searchword = ""
for word, cnt in dic1_count.items() :
    if cnt > 1 :
        searchWord = word
        print("    " + searchWord + "->" + str(cnt))
print()
print('5. 프로그램 종료문')
print('   print("Program End")')
print()
print('6. 프로그램 종료')
print("   Program End")
```

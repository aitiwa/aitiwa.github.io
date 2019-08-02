---
title:  "문자열 다루기 - 이름 문자열을 이용한 사례"
published: true
permalink: m3_1_forloopTest.html
summary: "This is forloopTest example for post.(m3_1_forloopTest)"
tags: [posts, news, getting_started, python, case_study]
sidebar: posts_sidebar
keywords: python, program, caseStudy, Dictionary
---
## Execution Result

**Hong Kil Dong, Hong Kil dong 등 동일 이름이 존재할 경우에 동일한 형태로 바꾸는 과정이다.**

## 문자열 다루기 - 이름 문자열을 이용한 사례

### 1. name, splitName 변수 선언과 초기화
```
name = "Hong Kil Dong"
splitName = ""        
```
### 2.1 프로그램본문-문자열 다루기 - 문자열 나누기
```
splitName = name.split(" ")
```
### 3.1 결과값 출력문
```
print(splitName)
```
### 4.1 결과값 출력
```
['Hong', 'Kil', 'Dong']
```
### 2.2 프로그램본문-문자열 다루기 - 특정 위치 영문자열 소문자변환
```
splitName[2] = splitName[2].replace(splitName[2][0], splitName[2][0].lower())
```
### 3.2 결과값 출력문
```
print(splitName[2])
```
### 4.2 결과값 출력
```
dong
```
### 2.3 프로그램본문-문자열 다루기 - 문자열 합치기
```
name = splitName[0] + " " + splitName[1].capitalize() + splitName[2]
```
### 3.3 결과값 출력문
```
print(name)
```
### 4.3 결과값 출력
```
Hong Kildong
```
### 2.4 프로그램본문-문자열 다루기 - 특정 영문자열 대문자변환
```
splitName[1].capitalize()
```
### 3.4 결과값 출력문
```
print(splitName[1].capitalize())
```
### 4.4 결과값 출력문
```
Kil
```
### 5.프로그램 종료문
```
  print("Program End")
```
### 6.프로그램 종료
```  
  Program End
```
## Program Source
```
print('caseStudy - 문자열 다루기 - 이름 문자열을 이용한 사례')
print('m3_1_forloopTest.py')
print()
print("1.name, splitName 변수 선언과 초기화")
print('name = "Hong Kil Dong"')
print('splitName = ""        ')
name = "Hong Kil Dong"
splitName = ""
print()
print("2.1프로그램본문-문자열 다루기 - 문자열 나누기")
print('splitName = name.split(" ")')
splitName = name.split(" ")
print()
print("3.1 결과값 출력문")
print('print(splitName)')
print()
print("4.1 결과값 출력")
print(splitName)
print()
print("2.2 프로그램본문-문자열 다루기 - 특정 위치 영문자열 소문자변환")
print('splitName[2] = splitName[2].replace(splitName[2][0], splitName[2][0].lower())')
splitName[2] = splitName[2].replace(splitName[2][0], splitName[2][0].lower())
print()
print("3.2 결과값 출력문")
print('print(splitName[2])')
print()
print("4.2 결과값 출력")
print(splitName[2])
print()
print("2.3 프로그램본문-문자열 다루기 - 문자열 합치기\n")
print('name = splitName[0] + " " + splitName[1].capitalize() + splitName[2]')
name = splitName[0] + " " + splitName[1].capitalize() + splitName[2]
print()
print("3.3 결과값 출력문")
print('print(name)')
print("4.3 결과값 출력")
print(name)
print()
print("2.4 프로그램본문-문자열 다루기 - 특정 영문자열 대문자변환\n")
print('splitName[1].capitalize()')
print()
print("3.4 결과값 출력문")
print('print(splitName[1].capitalize())')
print()
print("4.4 결과값 출력")
print(splitName[1].capitalize())
print()
print('5. 프로그램 종료')
print('   print("Program End")')
print('6. 프로그램 종료')
print("   Program End")
```

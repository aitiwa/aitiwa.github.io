---
title:  'caseStudy for_000: 반복문 기본형'
published: true
permalink: caseStudy_for_000.html
summary: "This is whileloopIfTest example for post.(whileloopIfTest)"
tags: [posts, news, getting_started, python, case_study]
sidebar: posts_sidebar
keywords: python, program, caseStudy, Dictionary
---

## Execution Result

## caseStudy for_000: 반복문 기본형

## 1. i 변수 선언과 초기화
```
   i  #암묵적 선언
```
## 2. 반복 출력하는 반복문
```
    for i in range(0,5):   #반복구문   
        if i%2 ==0 :                  
            print(str(i) + ': 짝수1')
        else:                         
            print(str(i) + ': 홀수1')
    print('--------')                 
    for i in range(0,5):   #반복구문  
        if i%2 ==0 :                 
            print('{}: 짝수2'.format(i))  
        else:                            
            print('{}: 홀수2'.format(i))  
```
## 3. 수행 결과값 출력
```
0: 짝수1
1: 홀수1
2: 짝수1
3: 홀수1
4: 짝수1
--------
0: 짝수2
1: 홀수2
2: 짝수2
3: 홀수2
4: 짝수2
```
## 4. 프로그램 종료문
```
   print("Program End")
```
## 5. 프로그램 종료
```
   Program End
```

## Program Source

```
print("caseStudy for_000: 반복문 기본형")
print()
print("1. i 변수 선언과 초기화 ")
print("   i  #암묵적 선언")
print()
print("2. 반복 출력하는 반복문 ")
print("    for i in range(0,5):   #반복구문   ")
print("        if i%2 ==0 :                  ")
print("            print(str(i) + ': 짝수1') ")
print("        else:                         ")
print("            print(str(i) + ': 홀수1') ")
print("    print('--------')                 ")
print("    for i in range(0,5):   #반복구문  ")
print("        if i%2 ==0 :                 ")
print("            print('{}: 짝수2'.format(i))  ")
print("        else:                            ")
print("            print('{}: 홀수2'.format(i))  ")
print()
print("3. 수행 결과값 출력")
for i in range(0,5):   #반복구문
    if i%2 ==0 :
        print(str(i) + ': 짝수1')
    else:
        print(str(i) + ': 홀수1')
print('--------')
for i in range(0,5):   #반복구문
    if i%2 ==0 :
        print('{}: 짝수2'.format(i))
    else:
        print('{}: 홀수2'.format(i))
print()
print('4. 프로그램 종료문')
print('   print("Program End")')
print()
print('5. 프로그램 종료')
print("   Program End")
```

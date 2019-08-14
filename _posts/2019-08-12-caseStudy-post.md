---
title:  '학점 계산 - 중첩 조건문 1단계'
published: true
permalink: ifElifElseMultiTest_001_01.html
summary: "This is ifElifElseMultiTest example for post.(ifElifElseMultiTest)"
tags: [posts, news, python, case_study]
sidebar: posts_sidebar
keywords: python, program, caseStudy
---

## Execution Result

**단순 학점을 조건에 따라 계산하고 출력한다.**

## caseStudy - 학점 계산 - 중첩 조건문 1단계

### 1. score 변수 선언과 초기화
```
   score = 95   
```
### 2. 여러 조건에 따라 실행하는 조건문
```
   if  score == 100 :               
       print("   A학점 입니다.")    
   elif score >=  90:               
       print("   A학점 입니다." )   
   elif score >= 80:                
       print("   B학점 입니다." )   
   elif score >= 70:                
       print("   C학점 입니다." )   
   elif score >= 60:                
       print("   D학점 입니다." )   
   else :                           
       print("   F학점 입니다." )   
```
### 3. 결과값->
```
   A학점 입니다.
```
### 4. 프로그램 종료문
```
   print("Program End")
```
###5. 프로그램 종료
```
   Program End
```   
## Program Source

```
print("caseStudy - 학점 계산 - 중첩 조건문 1단계")
print()
print("1. score 변수 선언과 초기화 ")
print('   score = 95   ')
score = 95
print()
print("2. 여러 조건에 따라 실행하는 조건문 및 출력문 ")
print('   if  score == 100 :               ')
print('       print("   A학점 입니다.")    ')
print('   elif score >=  90:               ')
print('       print("   A학점 입니다." )   ')
print('   elif score >= 80:                ')
print('       print("   B학점 입니다." )   ')
print('   elif score >= 70:                ')
print('       print("   C학점 입니다." )   ')
print('   elif score >= 60:                ')
print('       print("   D학점 입니다." )   ')
print('   else :                           ')
print('       print("   F학점 입니다." )   ')
print()
print("3. 결과값 출력")
if  score == 100 :
    print("   A학점 입니다.")
elif score >=  90:
    print("   A학점 입니다." )
elif score >= 80:
    print("   B학점 입니다." )
elif score >= 70:
    print("   C학점 입니다." )
elif score >= 60:
    print("   D학점 입니다." )
else :
    print("   F학점 입니다." )
print()
print('4. 프로그램 종료문')
print('   print("Program End")')
print()
print('5. 프로그램 종료')
print("   Program End")
```

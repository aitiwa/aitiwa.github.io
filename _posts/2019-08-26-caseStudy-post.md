---
title:  '학점 계산 - 중첩 조건문 5단계 - 0+ 중복 제거'
published: true
permalink: ifElifElseMultiTest_m3_1_05.html
summary: "This is ifelifelsemultiTest example for post.(ifelifelsemultiTest)"
tags: [posts, news, python, case_study]
sidebar: posts_sidebar
keywords: python, program, caseStudy
---

## Execution Result

**단순 학점을 조건에 따라 계산하고 출력한다. 0+학점 부여, 변수 입력, 0+ 중복 제거**

### caseStudy - 학점 계산 - 중첩 조건문 5단계 - 0+ 중복 제거

### 1. score 변수 선언과 입력받기
```
   score = int(input("   점수를 입력하세요:"))   
```
```   
   점수를 입력하세요:95
```   
### 2. 여러 조건에 따라 실행하는 조건문과 출력문
```
   if score >= 90:                   
       print("   A", end="")         
   elif 90> score >= 80:             
       print("   B", end="")         
   elif score >= 70:                 
       print("   C", end="")         
   elif score >= 60:                 
       print("   D", end="")         
   else:                             
       print("   F", end="")         

   if score == 100:                  
       print("+", end="")            
   elif score >=60:                  
       result = score % 10           
       if result < 5:                
           print("0", end="")        
       else:                         
           print("+", end="")   
```
### 3. 결과값 출력
```
   A+학점 입니다.
```   
### 4. 프로그램 종료문
```
   print("Program End")
```
### 5. 프로그램 종료
```
   Program End
```   
## Program Source

```
print("caseStudy - 학점 계산 - 중첩 조건문 5단계 - 0+ 중복 제거")
print()
print("1. score 변수 선언과 입력받기")
print('   score = int(input("   점수를 입력하세요:"))   ')
score = int(input("   점수를 입력하세요:"))
print("2. 여러 조건에 따라 실행하는 조건문과 출력문")
print('   if score >= 90:                   ')
print('       print("   A", end="")         ')
print('   elif 90> score >= 80:             ')
print('       print("   B", end="")         ')
print('   elif score >= 70:                 ')
print('       print("   C", end="")         ')
print('   elif score >= 60:                 ')
print('       print("   D", end="")         ')
print('   else:                             ')
print('       print("   F", end="")         ')
print('                                     ')
print('   if score == 100:                  ')
print('       print("+", end="")            ')
print('   elif score >=60:                  ')
print('       result = score % 10           ')
print('       if result < 5:                ')
print('           print("0", end="")        ')
print('       else:                         ')
print('           print("+", end="")        ')
print()
print("3. 결과값 출력")
if score >= 90:
    print("   A", end="")
elif 90> score >= 80:
    print("   B", end="")
elif score >= 70:
    print("   C", end="")
elif score >= 60:
    print("   D", end="")
else:
    print("   F", end="")

if score == 100:
    print("+", end="")
elif score >=60:
    result = score % 10
    if result < 5:
        print("0", end="")
    else:
        print("+", end="")

print("학점 입니다.")
print()
print('4. 프로그램 종료문')
print('   print("Program End")')
print()
print('5. 프로그램 종료')
print("   Program End")
```

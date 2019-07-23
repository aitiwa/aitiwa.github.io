---
layout: post
title: caseStudyProgram: 학점 계산 - 중첩 조건문 1단계 by python
subtitle: ifElifElseMultiTest_001_01.py
image: /img/hello_world.jpeg
tags: [python, program]
---

#실행결과

caseStudyProgram: 학점 계산 - 중첩 조건문 2단계 - 학점 입니다 중복 제거
m3_1_ifelifelsemultiTest_001_02.py

1. score 변수 선언과 초기화:

   score = 95   

2. 여러 조건에 따라 실행하는 조건문:

   if  score == 100 :               
       print("   A", end="")    
   elif score >=  90:               
       print("   A", end="" )   
   elif score >= 80:                
       print("   B", end="" )   
   elif score >= 70:                
       print("   C", end="" )   
   elif score >= 60:                
       print("   D", end="" )   
   else :                           
       print("   F", end="" )   

3. 결과값->

   A학점 입니다.

4. 프로그램 종료

   print("Program End")

   Program End

#Program Source

print("caseStudyProgram: 학점 계산 - 중첩 조건문 2단계 - 학점 입니다 중복 제거")
print('m3_1_ifelifelsemultiTest_001_02.py\n')
print("1. score 변수 선언과 초기화: ")
print('   score = 95   ')
score = 95
print()
print("2. 여러 조건에 따라 실행하는 조건문: ")
print('   if  score == 100 :               ')
print('       print("   A", end="")    ')
print('   elif score >=  90:               ')
print('       print("   A", end="" )   ')
print('   elif score >= 80:                ')
print('       print("   B", end="" )   ')
print('   elif score >= 70:                ')
print('       print("   C", end="" )   ')
print('   elif score >= 60:                ')
print('       print("   D", end="" )   ')
print('   else :                           ')
print('       print("   F", end="" )   ')
print()
print("3. 결과값->")
if  score == 100 :
    print("   A", end="")
elif score >=  90:
    print("   A", end="" )
elif score >= 80:
    print("   B", end="" )
elif score >= 70:
    print("   C", end="" )
else:
    print("F", end="")

print("학점 입니다.")

print()
print('4. 프로그램 종료')
print('   print("Program End")')
print("   Program End")

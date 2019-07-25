---
layout: post
title: caseStudy - 학점 계산 - 중첩 조건문 1단계
subtitle: ifElifElseMultiTest_001_01.py
image: /img/hello_world.jpeg
tags: [python, program,caseStudy]
---

#실행결과

caseStudyProgram: 학점 계산 - 중첩 조건문 1단계 by python
m3_1_ifElifElseMultiTest_001_01.py

1. score 변수 선언과 초기화:

   score = 100   

2. 여러 조건에 따라 실행하는 조건문:

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

3. 결과값->

   A학점 입니다.

4. 프로그램 종료

   print("Program End")
   Program End

#Program Source

print("caseStudyProgram: 학점 계산 - 중첩 조건문 1단계 by python")
print("m3_1_ifElifElseMultiTest_001_01.py\n")
print("1. score 변수 선언과 초기화: ")
print('   score = 100   ')
score = 95
print()
print("2. 여러 조건에 따라 실행하는 조건문: ")
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
print("3. 결과값->")
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
print('4. 프로그램 종료')
print('   print("Program End")')
print("   Program End")

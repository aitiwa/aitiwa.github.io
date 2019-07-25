---
layout: post
title: caseStudy - 반복문-문자열 읽어 오기-문자열을 "HelloKOREA" 이용한 사례
subtitle: m3_2_nestedLoopTest.py
image: /img/hello_world.jpeg
tags: [python, program,caseStudy]
---

#실행결과

caseStudy - DataType Dictionary 정의 - key/value, {}을 사용하는 자료형
study datatype_Dictionary_01.py

1.str1,result 변수 선언과 초기화

  str1 = "HelloKOREA"
  result = ""

2.문자열 함수와 반복 실행하는 반복문

  size = len(str1)  
  print("   문자열 길이: ",size)  
  print(str1)  

  for i in str1:  
      result  +=  i  
  print(result)  

  list1=list(str1)  
  for i in list1:  
      print(i, end = "")  

3.결과값->

  size = len(str1)
  print("   문자열 길이: ",size)  
  문자열 길이:  10
  print(" ",str1)
  HelloKOREA
  HelloKOREA
  H  e  l  l  o  K  O  R  E  A
  print("  ", list1)
  ['H', 'e', 'l', 'l', 'o', 'K', 'O', 'R', 'E', 'A']

4.프로그램 종료

  print("Program End")
  Program End

#Program Source

print("caseStudy - 반복문-문자열 읽어 오기")
print('study m3_1_forloopTest_003_002.py')
print()
print("1.str1,result 변수 선언과 초기화:  ")
print('  str1 = "HelloKOREA" ')
print('  result = "" ')
str1 = "HelloKOREA"
result = ""
print()
print("2.문자열 함수와 반복 실행하는 반복문 ")
print('  size = len(str1)  ')
print('  print("   문자열 길이: ",size)  ')
print('  print(str1)  ')
print(' ')
print('  for i in str1:  ')
print('      result  +=  i  ')
print('  print(result)  ')
print(' ')
print('  list1=list(str1)  ')
print('  for i in list1:  ')
print('      print(i, end = "")  ')
print()
print("3.결과값->")
print('  size = len(str1) ')
size = len(str1)
print('  print("   문자열 길이: ",size)  ')
print("  문자열 길이: ",size)
print('  print(" ",str1) ')
print(" ",str1)
for i in str1:
    result  +=  i
print(" ", result)

list1=list(str1)
for i in list1:
    print(" ", i, end = "")
print()
print('  print("  ", list1) ')
print(" ", list1)
print()
print('4.프로그램 종료')
print('  print("Program End")')
print("  Program End")

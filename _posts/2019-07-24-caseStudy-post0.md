---
layout: post
title: caseStudy - Section034 반복문을 이용한 화폐의 매수 계산
subtitle: m3_2_nestedLoopTest.py
image: /img/hello_world.jpeg
tags: [python, program,Section034,caseStudyProgram]
---

#실행결과

Section034 반복문을 이용한 화폐의 매수 계산 알고리즘
m3_2_nestedLoopTest.py

1.1 화폐 단위가 저장 될 변수 선언

   i = 50000
1.2 스위치 변수 선언: 다음번 계산할 금액 단위 결정

   SW = 0
1.3 금액을 입력받아 저장될 변수 선언

   j = int(input("   매수를 구할 금액을 입력하세요: "))

   매수를 구할 금액을 입력하세요: 65000

2. 입력된 금액을 계산해 실행할 반복문

   for l in range(1,11,1): # 1부터 시작, 11보다 작을 때까지, 1단위씩\n
       k = int(j/i) # 금액 단위 별 순차로 매수 계산\n
       print('   %5d %d ' % (int(i), k)) # 결과 출력\n
       j = j - (k*i) #금액 단위 순차로 계산해서 입력 받은 금액에서 뺀다.\n
       if SW == 0:  0이면 5, 1이면 2로 나눈다\n
          i = i/5\n  
          SW = 1\n
       else:\n
          i = i/2\n
          SW = 0\n

3. 결과값 출력 ->

   50000 1
   10000 1
    5000 1
    1000 0
     500 0
     100 0
      50 0
      10 0
       5 0
       1 0

4. 프로그램 종료

   print("Program End")

   Program End

#Program Source

print("Section034 반복문을 이용한 화폐의 매수 계산 알고리즘")
print("m3_2_nestedLoopTest.py")
print()
print("1.1 화폐 단위가 저장 될 변수 선언")
print("   i = 50000")
i = 50000
print("1.2 스위치 변수 선언: 다음번 계산할 금액 단위 결정")
print("   SW = 0")
SW = 0
print("1.3 금액을 입력받아 저장될 변수 선언")
print('   j = int(input("   매수를 구할 금액을 입력하세요: "))')
j = int(input("   매수를 구할 금액을 입력하세요: "))
print()
print("2. 입력된 금액을 계산해 실행할 반복문")
print("   for l in range(1,11,1): # 1부터 시작, 11보다 작을 때까지, 1단위씩")
print("       k = int(j/i) # 금액 단위 별 순차로 매수 계산")
print("       print('   %5d %d ' % (int(i), k)) # 결과 출력")
print("       j = j - (k*i) #금액 단위 순차로 계산해서 입력 받은 금액에서 뺀다.")
print('       if SW == 0:  0이면 5, 1이면 2로 나눈다')
print('          i = i/5  ')
print("          SW = 1 ")
print("       else: ")
print("          i = i/2 ")
print("          SW = 0")
print()
print("3. 결과값 출력 ->")
for l in range(1,11,1): # 1부터 시작, 11보다 작을 때까지, 1단위씩
    k = int(j/i)
    print('   %5d %d ' % (int(i), k))
    j = j - (k*i)
    if SW == 0:
        i = i/5
        SW = 1
    else:
        i = i/2
        SW = 0
print()
print('4. 프로그램 종료')
print('   print("Program End")')
print("   Program End")

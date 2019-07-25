---
layout: post
title: caseStudy - 반복문-문자열 읽어 오기-문자열을 "HelloKOREA" 이용한 사례
subtitle: m3_2_nestedLoopTest.py
image: /img/hello_world.jpeg
tags: [python, program,Section034,caseStudyProgram]
---

#실행결과

caseStudy - 반복문-문자열 읽어 오기-문자열을 "HelloKOREA" 이용한 사례
m3_2_forloopTest_003_003.py

1. 문자열 변수선언\n
   import operator    
   str1 = 'HelloKOREA'

2. 문자열 변수를 리스트 변수로 선언\n
   list1 = list(str1)

2.1 리스트 index 값 출력(위치확인)\n
   print(list1)
   결과-> ['H', 'e', 'l', 'l', 'o', 'K', 'O', 'R', 'E', 'A']

2.2 특정 문자열 값 출력\n
   print(list1[0])
   결과->  H

2.3 특정 문자열 값 출력\n
   print(list1[5])
   결과->  K

3. 리스트 변수의 딕셔너리 변수 선언\n
   dic1 = dict(zip(range(len(list1)),list1))

3.1 딕셔너리에서 index 값 출력(위치확인)\n
   print(dic1)
   결과-> {0: 'H', 1: 'e', 2: 'l', 3: 'l', 4: 'o', 5: 'K', 6: 'O', 7: 'R', 8: 'E', 9: 'A'}

4. 리스트에서 딕셔너리를 이용해 문자열 Key로 반복 숫자 계산\n
4.1 문자열 반복횟수용 딕셔너리 변수선언\n
   dic1_count = {}

4.2 문자열 반복횟수 계산하는 반복문 정의\n
    for i in list1: //리스트를 순차로 반복해서 실행\n
        if i not in dic1_count: //카운트에 문자열 Key값이 없으면\n
              dic1_count[i] = 1 //카운트 문자열 Key의 Value에 1을 지정하고\n
        else: //카운트에 문자열 Key값이 존재하면\n
              dic1_count[i] += 1 //카운트 문자열 Key의 Value에 1을 더한다.\n

4.3 결과값->\n
4.3.1 딕셔너리 카운트 기본 Key, Value 출력\n
   print(dic1_count)
   결과-> {'H': 1, 'e': 1, 'l': 2, 'o': 1, 'K': 1, 'O': 1, 'R': 1, 'E': 1, 'A': 1}

4.3.2 딕셔너리 카운트 Key, Value 출력\n
   print(dic1_count.items())
   결과-> dict_items([('H', 1), ('e', 1), ('l', 2), ('o', 1), ('K', 1), ('O', 1), ('R', 1), ('E', 1), ('A', 1)])

4.3.3 변수 유형 확인하기\n
   type(dic1_count)
   결과-> <class 'dict'>

5. 프로그램 종료\n
   print("Program End")\n
   Program End\n

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

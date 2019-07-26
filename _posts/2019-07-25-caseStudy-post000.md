---
layout: post
title: 반복문-문자열 읽어 오기-문자열을 "HelloKOREA" 이용한 사례
subtitle: study datatype_Dictionary_01.py
#image: /img/hello_world.jpeg
tags: [python, program, caseStudy]
---

#실행결과


caseStudy - 반복문-문자열 읽어 오기-문자열을 "HelloKOREA" 이용한 사례
m3_1_forloopTest.py

1.문자열 변수선언

   str1 = 'HelloKOREA'

2.문자열 변수를 리스트 변수로 선언

   list1 = list(str1)

3.리스트 변수의 딕셔너리 변수 선언

   dic1 = dict(zip(range(len(list1)),list1))

3.1 딕셔너리 index 값 출력(위치확인)

   print(dic1)

   결과->

   {0: 'H', 1: 'e', 2: 'l', 3: 'l', 4: 'o', 5: 'K', 6: 'O', 7: 'R', 8: 'E', 9: 'A'}

4.딕셔너리를 이용해 문자열 Key로 반복 숫자 계산

4.1 문자열 반복횟수용 딕셔너리 변수선언

   dic1_count = {}

4.2 딕셔너리에서 문자열 반복횟수 계산하는 반복문 정의


   for i in list1: //리스트를 순차로 반복해서 실행

       if i not in dic1_count: //카운트에 문자열 Key값이 없으면

             dic1_count[i] = 1 //카운트 문자열 Key의 Value에 1을 지정하고

       else: //카운트에 문자열 Key값이 존재하면

             dic1_count[i] += 1 //카운트 문자열 Key의 Value에 1을 더한다.

4.3 결과값->

4.3.1 딕셔너리 카운트 기본 Key, Value 출력

   print(dic1_count)

   결과->

   {'H': 1, 'e': 1, 'l': 2, 'o': 1, 'K': 1, 'O': 1, 'R': 1, 'E': 1, 'A': 1}

5.딕셔너리 정렬과 출력

5.1 딕셔너리 Key에 의한  정렬과 Key, Value 값 출력

   sortedlist11 = sorted(dic1_count.items())
   print(sortedlist11)

   결과->

   [('A', 1), ('E', 1), ('H', 1), ('K', 1), ('O', 1), ('R', 1), ('e', 1), ('l', 2), ('o', 1)]

   # items() 함수를 호출하면, key-value 쌍이 tuple로 구성된 리스트가 리턴된다.

5.2 딕셔너리 Key에 의한  정렬과 Key 값 출력

   sortedlist12 = sorted(dic1_count.keys())
   print(sortedlist12)


   결과->

   ['A', 'E', 'H', 'K', 'O', 'R', 'e', 'l', 'o']

5.3 딕셔너리 Key에 의한 정렬과 Key, Value 값 출력: 5.1, 5.2 참조

   sortedlist19 = sorted(dic1_count.items(),key=operator.itemgetter(0))
   print(sortedlist19)

   결과->

   [('A', 1), ('E', 1), ('H', 1), ('K', 1), ('O', 1), ('R', 1), ('e', 1), ('l', 2), ('o', 1)]

5.4 딕셔너리 Key에 의한 역정렬과 Key, Value 값 출력: 5.3 참조

   sortedlist15 = sorted(dic1_count.items(),key=operator.itemgetter(0),reverse=True)
   print(sortedlist15)

   결과->

   [('o', 1), ('l', 2), ('e', 1), ('R', 1), ('O', 1), ('K', 1), ('H', 1), ('E', 1), ('A', 1)]

5.5 딕셔너리 Value에 의한  정렬과 Value 값 출력

   sortedlist13 = sorted(dic1_count.values())
   print(sortedlist13)

   결과->

   [1, 1, 1, 1, 1, 1, 1, 1, 2]

5.6 딕셔너리 Value에 의한 정렬, 동일값 딕셔너리 Key 비정렬 및 Key, Value 값 출력: 5.5 참조

   sortedlist16 = sorted(dic1_count.items(),key=operator.itemgetter(1))
   print(sortedlist16)

   결과->

   [('H', 1), ('e', 1), ('o', 1), ('K', 1), ('O', 1), ('R', 1), ('E', 1), ('A', 1), ('l', 2)]

5.7 딕셔너리 Value에 의한 정렬, 동일값 Key에 의한 정렬 및 Key, Value 값 출력

   sortedlist20 = sorted(dic1_count.items(),key=operator.itemgetter(1,0))

   결과->

   [('A', 1), ('E', 1), ('H', 1), ('K', 1), ('O', 1), ('R', 1), ('e', 1), ('o', 1), ('l', 2)]

5.8 딕셔너리 Value에 의한 역정렬, 동일값 딕셔너리 Key 비정렬 및 Key, Value 값 출력: 5.6 참조

   sortedlist14 = sorted(dic1_count.items(),key=operator.itemgetter(1),reverse=True)
   print(sortedlist14)

   결과->

   [('l', 2), ('H', 1), ('e', 1), ('o', 1), ('K', 1), ('O', 1), ('R', 1), ('E', 1), ('A', 1)]

5.9 딕셔너리 Value에 의한 역정렬과 동일값 딕셔너리 Key역정렬 및 Key, Value 값 출력: 5.7 참조

   sortedlist18 = sorted(dic1_count.items(),key=operator.itemgetter(1,0),reverse=True)
   print(sortedlist18)

   결과->

   [('l', 2), ('o', 1), ('e', 1), ('R', 1), ('O', 1), ('K', 1), ('H', 1), ('E', 1), ('A', 1)]

5.10 변수의 데이터유형

   type(sortedlist18)

   결과->

   <class 'list'>

5.11 정렬한 리스트 변수의 값을 문자열로 출력1

   for i in sortedlist18: //문자열을 순차 반복으로 실행

       print('{}{}'.format(i[0],i[1]),end='') //문자열 양식으로 출력


   결과->

   l2o1e1R1O1K1H1E1A1

5.12 정렬한 리스트 변수의 값을 문자열로 출력2

   문자열 변수 선언

   strList19 = ""
   for i in sortedlist18: //문자열을 순차 반복으로 실행

       strList19 += i[0] + str(i[1]) //문자열 합치기


   결과->

   print(strList19)

   l2o1e1R1O1K1H1E1A1

   l2

6.프로그램 종료

   print("Program End")

   Program End

#Program Source

print('caseStudy - 반복문-문자열 읽어 오기-문자열을 "HelloKOREA" 이용한 사례')
print('m3_1_forloopTest.py')
import operator
print("1. 문자열 변수선언: ")
print("   str1 = 'HelloKOREA'")
str1 = "HelloKOREA"
print()
print("2. 문자열 변수를 리스트 변수로 선언: ")
print("   list1 = list(str1)")
list1 = list(str1)
print()
print("3. 리스트 변수의 딕셔너리 변수 선언: ")
print("   dic1 = dict(zip(range(len(list1)),list1))")
dic1 = dict(zip(range(len(list1)),list1))
print()
print("3.1 딕셔너리 index 값 출력(위치확인): print(dic1)")
print("   print(dic1)")
print("   결과->",dic1)
print()
print("4. 딕셔너리를 이용해 문자열 Key로 반복 숫자 계산")
print("4.1 문자열 반복횟수용 딕셔너리 변수선언:")
print("   dic1_count = {}")
dic1_count = {}
print()
print("4.2 딕셔너리에서 문자열 반복횟수 계산하는 반복문 정의")
print("   for i in list1: //리스트를 순차로 반복해서 실행")
print("       if i not in dic1_count: //카운트에 문자열 Key값이 없으면")
print("             dic1_count[i] = 1 //카운트 문자열 Key의 Value에 1을 지정하고")
print("       else: //카운트에 문자열 Key값이 존재하면")
print("             dic1_count[i] += 1 //카운트 문자열 Key의 Value에 1을 더한다.")
print()
for i in list1:
     if i not in dic1_count.keys():
        dic1_count[i] = 1
     else:
        dic1_count[i] += 1
print("4.3 결과값->")
print("4.3.1 딕셔너리 카운트 기본 Key, Value 출력:")
print("   print(dic1_count)")
print("   결과->", dic1_count)
print()
print("5. 딕셔너리 정렬과 출력")
print("5.1 딕셔너리 Key에 의한  정렬과 Key, Value 값 출력")
print("   sortedlist11 = sorted(dic1_count.items())")
sortedlist11 = sorted(dic1_count.items())
print("   print(sortedlist11)")
print("   결과->", sortedlist11)
print("   * items() 함수를 호출하면, key-value 쌍이 tuple로 구성된 리스트가 리턴된다.")
print("5.2 딕셔너리 Key에 의한  정렬과 Key 값 출력: ")
print("   sortedlist12 = sorted(dic1_count.keys())")
sortedlist12 = sorted(dic1_count.keys())
print("   print(sortedlist12)")
print("   결과->", sortedlist12)
print("5.3 딕셔너리 Key에 의한 정렬과 Key, Value 값 출력: 4.1, 4.2 참조 ")
print("   sortedlist19 = sorted(dic1_count.items(),key=operator.itemgetter(0))")
sortedlist19 = sorted(dic1_count.items(),key=operator.itemgetter(0))
print("   print(sortedlist19)")
print("   결과->",sortedlist19)
print("5.4 딕셔너리 Key에 의한 역정렬과 Key, Value 값 출력: 4.3 참조 ")
print("   sortedlist15 = sorted(dic1_count.items(),key=operator.itemgetter(0),reverse=True)")
sortedlist15 = sorted(dic1_count.items(),key=operator.itemgetter(0),reverse=True)
print("   print(sortedlist15)")
print("   결과->",sortedlist15)
print("5.5 딕셔너리 Value에 의한  정렬과 Value 값 출력: ")
print("   sortedlist13 = sorted(dic1_count.values())")
sortedlist13 = sorted(dic1_count.values())
print("   print(sortedlist13)")
print("   결과->", sortedlist13)
print("5.6 딕셔너리 Value에 의한 정렬, 동일값 딕셔너리 Key 비정렬 및 Key, Value 값 출력: 4.5 참조")
print("   sortedlist16 = sorted(dic1_count.items(),key=operator.itemgetter(1))")
sortedlist16 = sorted(dic1_count.items(),key=operator.itemgetter(1))
print("   print(sortedlist16)")
print("   결과->",sortedlist16)
print("5.7 딕셔너리 Value에 의한 정렬, 동일값 Key에 의한 정렬 및 Key, Value 값 출력: ")
print("   sortedlist20 = sorted(dic1_count.items(),key=operator.itemgetter(1,0))")
sortedlist20 = sorted(dic1_count.items(),key=operator.itemgetter(1,0))
print("   결과->",sortedlist20)
print("5.8 딕셔너리 Value에 의한 역정렬, 동일값 딕셔너리 Key 비정렬 및 Key, Value 값 출력: 4.6 참조")
print("   sortedlist14 = sorted(dic1_count.items(),key=operator.itemgetter(1),reverse=True)")
sortedlist14 = sorted(dic1_count.items(),key=operator.itemgetter(1),reverse=True)
print("   print(sortedlist14)")
print("   결과->",sortedlist14)
print("5.9 딕셔너리 Value에 의한 역정렬과 동일값 딕셔너리 Key역정렬 및 Key, Value 값 출력: 4.7 참조")
print("   sortedlist18 = sorted(dic1_count.items(),key=operator.itemgetter(1,0),reverse=True)")
sortedlist18 = sorted(dic1_count.items(),key=operator.itemgetter(1,0),reverse=True)
print("   print(sortedlist18)")
print("   결과->",sortedlist18)
print("5.10 변수의 데이터유형: ")
print("   type(sortedlist18)")
print("   결과->",type(sortedlist18))
print("5.11 정렬한 리스트 변수의 값을 문자열로 출력1: ")
print("   for i in sortedlist18: //문자열을 순차 반복으로 실행")
print("       print('{}{}'.format(i[0],i[1]),end='') //문자열 양식으로 출력")
print("   결과->")
for i in sortedlist18:
    print("{}{}".format(i[0],i[1]),end="")
print()
print("5.12 정렬한 리스트 변수의 값을 문자열로 출력2: ")
print("   문자열 변수 선언: ")
print('   strList19 = "" ')
strList19 = ""
print("   for i in sortedlist18: //문자열을 순차 반복으로 실행")
print("       strList19 += i[0] + str(i[1]) //문자열 합치기")
for i in sortedlist18:
    strList19 += i[0] + str(i[1])
print("   결과->")
print('   print(strList19)')
print(strList19)
print()
maxCnt = 0
for j, cnt in dic1_count.items() :
    if maxCnt < cnt :
        maxCnt = cnt
        searchword = j
print(searchword + str(maxCnt))
print()
print('6. 프로그램 종료')
print('   print("Program End")')
print("   Program End")

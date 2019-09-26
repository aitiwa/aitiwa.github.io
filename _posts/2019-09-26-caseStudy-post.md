---
title:  '문자열 다루기 - "HelloKOREA" 리스트로 전환 사례2'
published: true
permalink: M3_ex03_evenPrint_004.html
summary: "This is whileloopIfTest example for post.(whileloopIfTest)"
tags: [posts, news, getting_started, python, case_study]
sidebar: posts_sidebar
keywords: python, program, caseStudy, Dictionary
---

## Execution Result

## caseStudy: 알고리즘 활용-10부터 0까지 커피 재고를 출력

## 1. coffee, money 변수 선언과 초기화
```
   coffee = 10
   money = 300
```
## 2. 반복 실행하는 반복문
```
    while money:  
        print("   돈을 받고 커피를 줍니다.")  
        coffee = coffee -1  
        print("   남은 커피의 양은 %d개입니다." % coffee)  
        if coffee == 0:  
            print("   커피가 다 떨어졌습니다. 판매를 중지합니다.")  
            break  
```
## 3. 결과값 출력
```
   돈을 받고 커피를 줍니다.
   남은 커피의 양은 9개입니다.
   돈을 받고 커피를 줍니다.
   남은 커피의 양은 8개입니다.
   돈을 받고 커피를 줍니다.
   남은 커피의 양은 7개입니다.
   돈을 받고 커피를 줍니다.
   남은 커피의 양은 6개입니다.
   돈을 받고 커피를 줍니다.
   남은 커피의 양은 5개입니다.
   돈을 받고 커피를 줍니다.
   남은 커피의 양은 4개입니다.
   돈을 받고 커피를 줍니다.
   남은 커피의 양은 3개입니다.
   돈을 받고 커피를 줍니다.
   남은 커피의 양은 2개입니다.
   돈을 받고 커피를 줍니다.
   남은 커피의 양은 1개입니다.
   돈을 받고 커피를 줍니다.
   남은 커피의 양은 0개입니다.
   커피가 다 떨어졌습니다. 판매를 중지합니다.
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
print("caseStudy: 알고리즘 활용-10부터 0까지 커피 재고를 출력")
print()
print("1. coffee, money 변수 선언과 초기화")
print('   coffee = 10 ')
print('   money = 300 ')
coffee = 10
money = 300
print()
print("2. 반복 실행하는 반복문 ")
print('    while money:  ')
print('        print("   돈을 받고 커피를 줍니다.")  ')
print('        coffee = coffee -1  ')
print('        print("   남은 커피의 양은 %d개입니다." % coffee)  ')
print('        if coffee == 0:  ')
print('            print("   커피가 다 떨어졌습니다. 판매를 중지합니다.")  ')
print('            break  ')
print()
print("3. 결과값 출력")
while money:
    print("   돈을 받고 커피를 줍니다.")
    coffee = coffee -1
    print("   남은 커피의 양은 %d개입니다." % coffee)
    if coffee == 0:
        print("   커피가 다 떨어졌습니다. 판매를 중지합니다.")
        break
print()
print('4. 프로그램 종료문')
print('   print("Program End")')
print()
print('5. 프로그램 종료')
print("   Program End")
```

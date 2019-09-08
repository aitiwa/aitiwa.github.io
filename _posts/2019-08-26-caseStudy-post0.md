---
title:  'Dictionary구조는 어떻게 사용 할까요?'
published: true
permalink: Dictionary_20190908.html
summary: "This is example for post.(Dictionary)"
tags: [posts, news, python, case_study, stage]
sidebar: posts_sidebar
keywords: python, program, caseStudy, Stage
---

## Execution Result

**Dictionary구조는 Key와 Value의 Set로 구성된다.**

### stage - Dictionary구조는 어떻게 사용 할까요?

### 1. Dictionary 변수 선언문
```
   people = {'korean': 380, 'american': 42, 'japanese': 15}
```
### 2. Dictionary 변수 출력문
```
   print("  ", people)
```
### 3. Dictionary 변수 출력값
```
   {'korean': 380, 'american': 42, 'japanese': 15}
```
### 4. Dictionary 변수 특정 위치 출력문
```
   print('  ', people['korean'])
```
### 5. Dictionary 변수 출력값
```
   380
```
### 6. Dictionary 변수의 특정 Key의 value 값 변경은 어떻게 할까요?
```
   people['american'] = 63
```
### 7. Dictionary 변수 출력값
```
   print('  ', people['american'])
   63

   print('  ', people['japanese'])
   15
```
### 8. Dictionary에 새로운 값(특정 Key, value 값) 추가는 어떻게 할까요?
```
   people['german'] = 29
```
### 9. Dictionary 변수 출력문
```
   print('  ', people)
```
### 10. Dictionary 변수 출력값
```
   {'korean': 380, 'american': 63, 'japanese': 15, 'german': 29}
```   
### 11. 프로그램 종료문
```
   print("Program End")
```
### 12. 프로그램 종료
```
   Program End
```   
## Program Source

```
print('stage - Dictionary구조는 어떻게 사용 할까요?')
print()
print('1. Dictionary 변수 선언문')
print("   people = {'korean': 380, 'american': 42, 'japanese': 15}")
people = {'korean': 380, 'american': 42, 'japanese': 15}
print()
print('2. Dictionary 변수 출력문')
print('   print("  ", people)')
print()
print('3. Dictionary 변수 출력값')
print("  ", people)
print()
print('4. Dictionary 변수 특정 위치 출력문')
print("   print('  ', people['korean'])")
print()
print('5. Dictionary 변수 출력값')
print('  ', people['korean'])
print()
print('6. Dictionary 변수의 특정 Key의 value 값 변경은 어떻게 할까요?')
print("   people['american'] = 63")
people['american'] = 63
print()
print('7. Dictionary 변수 출력값')
print("   print('  ', people['american'])")
print('  ', people['american'])
print()
print("   print('  ', people['japanese'])")
print('  ', people['japanese'])
print()
print('8. Dictionary에 새로운 값(특정 Key, value 값) 추가는 어떻게 할까요?')
print("   people['german'] = 29")
people['german'] = 29
print()
print('9. Dictionary 변수 출력문')
print("   print('  ', people)")
print()
print('10. Dictionary 변수 출력값')
print('  ', people)
```

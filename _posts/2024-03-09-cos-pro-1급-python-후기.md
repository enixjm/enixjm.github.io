---
layout: post
title: COS PRO 1급 파이썬 후기
categories: etc
excerpt_image: https://github.com/enixjm/enixjm.github.io/assets/30498334/7655680d-c6c9-4cbf-8f0a-3126bec9650e
---
## 코딩전문가자격시험, COS Pro(Professional Coding Specialist) 
 - [C, C++, C#, JAVA, Python] 언어 지원
 - CBT 환경 (Programmers와 유사)
 - SW 개발병 자격증 기사 이상 급 부여 (10점/10점)

##### COS PRO 과목별 응시료 할인 쿠폰
> [https://www.ybmit.com/event/revent/2024/0201/event.jsp](https://www.ybmit.com/event/revent/2024/0201/event.jsp)

2024년도에 시험을 보실 예정이시라면 3월 이내로 미리 할인 쿠폰을 받아두시면 좋겠습니다.
![image](https://github.com/enixjm/enixjm.github.io/assets/30498334/7655680d-c6c9-4cbf-8f0a-3126bec9650e){: height="250"}

---

## 1급 난이도 및 유형
> [Solved.ac](https://solved.ac/problems/level){:target="_blank"}

Solved 기준 **[실버 1~ 골드 3]** 수준이고 평균적으로 골드 5정도의 난이도로 체감되었습니다. 빈칸 채우기와 한줄 바꾸기, 구현으로 이루어 진것을 감안하면 이것보다 조금 더 낮은 난이도로 봐도 되겠습니다.
DFS,BFS나 간단한 DP 수준의 알고리즘은 이해하고 있어야하며 COS Pro에서는 특히 문자열 처리가 자주 출제되는 것 같습니다. 때문에 문자열 처리를 알고가시고 Python으로 응시하신다면 더 유리할 것 같습니다. 

## 문제 유형
**샘플 문제보다 훨신 어렵습니다!**  
[ 코드이해(빈 칸 채우기), 디버깅(한 줄 바꾸기), 설계(함수 작성) ] 세 부분으로 나누어져 있습니다.
배점이 문제당 100점으로 동일하지 않고 구현이나 빈칸채우기 부분이 배점이 큽니다.  
  
#### 기억나는 몇 문제들입니다.
**1번. 문자열 특수문자 제거 및 대소문자 구분 (빈칸채우기)**  
리스트 컴프리헨션 코드와 string 내장함수를 이용하여 특수문자를 제거한 문자열, 소문자만 있는 문자열, 대문자만 있는 문자열을 출력하는 문제입니다. isalpha() 또는 isalnum()을 이용하여 특수문자를 제거하고 lower()와 upper() 함수로 대소문자 문자열을 만드는 것인데 특수문자 제거하는 함수가 기억나지 않아 틀리고 말았습니다.   
   

**2번. 동전 거스르기 (빈칸 채우기)**  
동전의 종류와 돈이 주어지면 동전 개수를 최소한으로 사용한 동전 수를 출력하는 문제입니다. 직접 작성한다면 금방 풀었겠지만 필기는 커녕 텍스트 메모조차 못하는 환경에서 머리로 코드를 굴리느라 시간을 많이 뺏겼습니다.   
   

**3번. 세 수의 최대 공약수 (빈칸 채우기)**     
세 수의 최대 공약수를 구하는 문제입니다.   
   
**10번. 셔틀버스 (함수 작성)**  
2018 카카오 블라인드 테스트 문제와 완전히 동일했습니다.
> https://school.programmers.co.kr/learn/courses/30/lessons/17678

## 시험 환경
![image](https://github.com/enixjm/enixjm.github.io/assets/30498334/599e8fa4-c744-4168-999f-1581b157fb07)
시험환경은 프로그래머스와 매우 유사합니다. 
코드 실행이 가능하지만 펜이나, 텍스트 메모 마저 사용할 수 없는 환경이기 때문에 유의하셔야 합니다.

## 후기
![image](https://github.com/enixjm/enixjm.github.io/assets/30498334/31225a59-d99d-4055-be71-254052164a63)
만만하게 보고 샘플 문제 몇개만 풀고 시험보다가 혼났습니다. 빈칸 채우기 문제에서 탈탈 털리고 몇 년 손 놓아 녹슨 알고리즘 실력을 제대로 체감하여 정신차리게 해주는 계기가 되었습니다.
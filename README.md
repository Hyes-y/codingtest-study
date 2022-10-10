# 공부하는 아이스베어 코테스터디

## 목표

- 매주 2개의 카테고리([백준 단계별로 풀기](https://www.acmicpc.net/step)) 안에서 문제 5개씩 풀기
- 매주 월요일 8시에 스터디 모임
  1. 코드 공유 (약 30분)
     - 모든 문제를 최대한 공유하도록 하되, 카테고리에 속한 문제가 지나치게 많은 경우 어려웠던 문제를 선정해서 공유함.
  2. 랜덤으로 고른 문제 1개를 다같이 풀고, 푼 방법 공유 (약 30분)
     - [프로그래머스 고득점 Kit](https://school.programmers.co.kr/learn/challenges?tab=algorithm_practice_kit)에서 랜덤으로 결정함.

## 기간

2022.08.08 ~ 

## 기록

### 0808 

- 카테고리: [재귀](https://www.acmicpc.net/step/19), [브루트 포스](https://www.acmicpc.net/step/22)
- 랜덤문제: 재귀의 [하노이 탑 이동순서](https://www.acmicpc.net/problem/11729)

### 0815 

> 공휴일에도 스터디하는 사람 성공한대요~

- 카테고리: [정렬](https://www.acmicpc.net/step/9), [집합과 맵](https://www.acmicpc.net/step/49)
- 랜덤문제: [해시](https://school.programmers.co.kr/learn/courses/30/parts/12077)의 [베스트 앨범](https://school.programmers.co.kr/learn/courses/30/lessons/42579)


### 0822

- 카테고리: [백트랙킹](https://www.acmicpc.net/step/34), [동적계획법1](https://www.acmicpc.net/step/16)
  - 출제 빈도를 고려하여(~~스터디원 뇌피셜~~) 기하1과 정수론과 조합론은 스터디에서 진행하지 않기로 함.
  - 의논한 문제
    - [N-queen](https://www.acmicpc.net/problem/9663)
      - 힌트: 충돌하지 않게 위치시키려면 같은 행 또는 열을 배제해야 하기때문에, 1차원배열에 저장해도 된다(2차원 배열이 없어도 표현 가능하다.)
        - 예를 들어, ```[0, 2, 3, 1]```는 1행 2열, 2행 3열, 3행 1열에 퀸이 위치한다는 의미.
    - [포도주 시식](https://www.acmicpc.net/problem/2156)
      - 계단 오르기와 비슷하지만 시작점과 끝점이 없다는 것이 다르다.
      - 해결 못한 반례 (해결했다면 '질문'채널에 설명 남겨주기~)
        ```
        답 : 36
        Input:
        10
        0
        0
        10
        0
        5
        10
        0
        0
        1
        10
        ```
- 랜덤문제: [스택/큐](https://school.programmers.co.kr/learn/courses/30/parts/12081)의 [같은 숫자는 싫어](https://school.programmers.co.kr/learn/courses/30/lessons/12906)
  - 다들 푼 방식이 비슷하고, 배열이나 큐를 사용해서 풀었다.
  - 프로그래머스에서 파이써닉하게 푼 것도 신기했음 
    ```python
    return  [arr[i] for i in range(len(arr)) if not(arr[i:i+1] == arr[i+1:i+2])]
    ```
  - 자바스크립트로 filter를 사용해서 한 줄에 나타낸 코드가 있었음
    ```javascript
    return arr.filter((val,index) => val != arr[index+1]);
    ```


### 0829

- 카테고리: [누적합](https://www.acmicpc.net/step/48), [그리디 알고리즘](https://www.acmicpc.net/step/33)
  - 의논한 문제
    - [나머지 합](https://www.acmicpc.net/problem/10986)
      - 힌트: 누적 합의 나머지를 구하고 그 값이 같은 것끼리 그룹을 형성한다. 각 그룹에서 2개를 고르면(조합) 범위가 형성된다. 나머지가 같기 때문에 두 값의 차가 0이라서, 최종적으로 누적합을 M으로 나누면 0이 된다.
- 랜덤문제: [힙](https://school.programmers.co.kr/learn/courses/30/parts/12117)의 [더 맵게](https://school.programmers.co.kr/learn/courses/30/lessons/42626)
  - 모두 [heapq](https://docs.python.org/ko/3/library/heapq.html) 사용해서 문제를 풀었다.
  - 우성님이 소개해 준 함수
    - [all(iterable)](https://docs.python.org/ko/3/library/functions.html?highlight=all#all): iterable 요소가 모두 참이면 True 반환
    - [any(iterable)](https://docs.python.org/ko/3/library/functions.html?highlight=all#any): iterable 요소가 하나라도 참이면 True 반환


### 0905

- 카테고리: [스택](https://www.acmicpc.net/step/11), [큐, 덱](https://www.acmicpc.net/step/12)
  - 의논한 문제
    - [스택 수열](https://www.acmicpc.net/problem/1874)
    - [오큰수](https://www.acmicpc.net/problem/17298)
- 랜덤문제: [정렬](https://school.programmers.co.kr/learn/courses/30/parts/12198)의 [가장 큰 수](https://school.programmers.co.kr/learn/courses/30/lessons/42746)


#### 0912 

- 추석연휴로 쉬어가기


### 0919

- 카테고리: [분할정복](https://www.acmicpc.net/step/20), [이분탐색](https://www.acmicpc.net/step/29)
  - 의논한 문제
    - [랜선 자르기](https://www.acmicpc.net/problem/1654): 각 랜선을 특정 개수로 똑같이 자를 때 최대 길이 구하기
    - [행렬제곱](https://www.acmicpc.net/problem/10830)
      - 4시간을 투자한 혜선님의 조언: 나머지를 구하는 문제인데 시간초과를 만났다면 ⭐ 모듈러 연산 ⭐ 사용하기
        1. (a + b) mod n = ((a mod n) + (b mod n)) mod n
        2. (a - b) mod n = ((a mod n) - (b mod n)) mod n
        3. (a * b) mod n = ((a mod n) * (b mod n)) mod n
      - [곱셈](https://www.acmicpc.net/problem/1629)이랑 유사하다.
- 랜덤문제: [완전탐색](https://school.programmers.co.kr/learn/courses/30/parts/12230)의 [모음사전](https://school.programmers.co.kr/learn/courses/30/lessons/84512)

### 0926

- 카테고리: [우선순위 큐](https://www.acmicpc.net/step/13), [동적계획법2](https://www.acmicpc.net/step/17)
- 랜덤문제: [탐욕법](https://school.programmers.co.kr/learn/courses/30/parts/12244)의 [조이스틱](https://school.programmers.co.kr/learn/courses/30/lessons/42860)
  - 아무도 못 풀었다🥲. 알파벳보다는 이동횟수 계산이 이 문제의 핵심인것 같다.
 
### 1003

- 카테고리: [동적계획법1](https://www.acmicpc.net/step/16), [동적계획법2](https://www.acmicpc.net/step/17)
- 랜덤문제: [동적계획법](https://school.programmers.co.kr/learn/courses/30/parts/12263)의 [사칙연산](https://school.programmers.co.kr/learn/courses/30/lessons/1843) 
  - 아무도 못 풀었다🥲. 다음주 스터디 시간까지 풀거나 공부해서 설명하기로 함.
  
### 1010

- 지난 주에 못푼 문제 사칙연산 풀이방법 의논
  - [1안: 2차원 배열에서 해결](https://school.programmers.co.kr/questions/35224)
  - [2안: 1차원 배열에서 해결](https://tiktaek.tistory.com/33)
- 카테고리: [그래프와 순회](https://www.acmicpc.net/step/24)
  - [뱀과 사다리 게임](https://www.acmicpc.net/problem/16928)
  - JS로 문제 풀 때 자료구조 Map을 사용해서 풀었음
    - [JS에서 Set, Map, Object 차이](https://velog.io/@proshy/JSSet-Map-Object-%EC%A0%95%EB%A6%AC)
  - 파이썬으로 dfs 문제 풀 때, 재귀호출 제한을 따로 설정해야 했음. (Python3 기준으로 최대 재귀 깊이는 1000)
    ```python
    import sys

    sys.setrecursionlimit(10 ** 9)
    ```
  - dfs 문제 풀 때, 재귀 또는 스택으로 푸는 방법이 있음
- 랜덤문제: [깊이/너비 우선탐색(DFS/BFS)](https://school.programmers.co.kr/learn/courses/30/parts/12421)의 [네트워크](https://school.programmers.co.kr/learn/courses/30/lessons/43162) 
  - 다른 팀원이 시도한 방식을 듣고 혜선님이 [유니온 파인드 알고리즘](https://ip99202.github.io/posts/%EC%9C%A0%EB%8B%88%EC%98%A8-%ED%8C%8C%EC%9D%B8%EB%93%9C(Union-Find)/)을 떠올렸음

### 1017

- 카테고리: [최단경로](https://www.acmicpc.net/step/26)
- 랜덤문제: [이분탐색](https://school.programmers.co.kr/learn/courses/30/parts/12486)의 [입국심사](https://school.programmers.co.kr/learn/courses/30/lessons/43238)

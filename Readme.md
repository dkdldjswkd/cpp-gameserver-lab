C++와 네트워크 관련 개념을 공부하며 구현한 프로젝트 모음입니다.  
각 프로젝트는 학습목적 또는 [락프리 게임서버 프로젝트](https://github.com/dkdldjswkd/lockfree-gameserver-core-cpp)를 위해 작성된 코드로서,  
네트워크, 자료구조, 알고리즘 등의 다양한 주제를 다룹니다.

## 주요 프로젝트

### 1. **AsyncSelect 그림판 (AsyncSelect I/O 모델을 사용한 비동기 I/O 처리)**
   `AsyncSelect` I/O 모델을 사용한 그림판 서버/클라이언트 프로젝트입니다.  
   클라이언트가 그리는 그림을 서버에 연결된 클라이언트에게 브로드 캐스트 합니다.

### 2. **A* (A 스타 알고리즘)**
   최단 경로를 찾는 알고리즘인 A* 알고리즘을 구현했습니다.
   A* 알고리즘은 출발 지점에서 목적 지점까지 가는 과정에서 새로운 지점을 Priority Queue에 추가하고, 가장 우선순위가 높은 지점부터 탐색을 반복하는 길찾기 알고리즘 입니다.

### 3. **JPS (Jump Point Search)**
   A* 알고리즘을 개선한 JPS 알고리즘을 구현한 예제입니다.  
   A*는 인접한 모든 지점을 Priority Queue에 추가하는 반면, JPS는 충돌 정보를 기반으로 중요한 분기점만 Priority Queue에 추가하여 탐색 거리가 멀수록 A*보다 더 빠른 경로 탐색 성능을 보입니다.  
<video width="640" height="360" controls>
  <source src="https://raw.githubusercontent.com/dkdldjswkd/SimplePoject/main/CppProject/22.09.05%20-%20JPS/JPS.mp4" type="video/mp4">
</video>

### 4. **LockFreeStack (락프리 스택)**
   락프리 스택을 구현하여 다중 스레드 환경에서도 성능 저하 없이 효율적으로 동작하는 자료구조를 제공합니다. 이를 통해 메모리 할당 경합을 최소화하고, 안정적인 멀티스레딩 환경을 구축할 수 있습니다.

### 5. **MMO TCPFighter Server**
   `select` I/O 모델을 사용한 간단한 MMO 프로젝트입니다.

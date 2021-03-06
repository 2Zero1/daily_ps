### 문제
더블 링크드 리스트로 만든 스택 2개를 이용하여 큐를 만든다.

실행 확인 방법
- enqueue(1)
- enqueue(2)
- enqueue(3)
- dequeue()->1
- dequeue()->2
- enqueue(4)
- dequeue()->3
- dequeue()->4

---



#### 1. 이해
미지의 것. 주어진 자료. 주어진 조건.
- 더블 링크드 리스트로 만든 스택 2개를 이용하면 된다.
- 더블 링크드 리스트에 필요한 모든 기능을 구현해야할까? 위 과제를 만들기 위한 수준으로만 구현해야할까?
- 큐는 FIFO(First In First Out)으로 먼저 들어온 요소가 먼저 나간다.
- 그러나 스택은 LIFO으로 가장 마지막에 들어온 요소가 먼저 나간다.

#### 2. 계획
- 스택에 123이 들어온다면 321 순으로 나간다. 스택에 123을 넣었을 때 123 순으로 나오게 하려면?
- 스택이 2개이기 때문에 enqueue용 스택과 dequeue용 스택을 나눠서 쓰면 될 것이다.
- enqueueStack에 1,2,3이 들어오고 dequeueStack에 dequeue()하면 enqueueStack->dequeueStack으로 element를 모두 옮긴다. 
- dequeue() 할 때 dequeueStack이 비어있는 상태라면 enqueueStack의 element를 모두 옮긴다.
- 필요한 메소드는 dequeue(), enqueue(), isEmpty().
- 우선 javascript의 array를 이용해서 각 stack을 구현하고 추후에 해당 stack을 더블 링크드 리스트로 구현한 stack으로 교체하도록 한다. 

#### 3. 실행
- 커밋 로그(https://github.com/wholemann/daily_ps/commits/master)

#### 4. 반성
- 비교적 무난하게 구현된 것 같다.
- 확실히 저번주보다 TDD 방식의 접근이 익숙해졌다.(어제 오프라인에서 피드백 받은게 효과를 본 듯. 역시 피드백 필수.)
- 내일은 array로 stack 구현한 다음 doublylinkedlist 교체하는 방식이 아닌 처음부터 doublylinkedlist를 만들자.
- 아직 describe에 들어간 문구를 어떻게 해야될지 잘 모르겠다. test code 리팩토링은 좀 더 연구를 해봐야 될 듯.

### 문제1
주어진 정수를 문자열로 변환한다.
ex) 1234 => '1234'

---

#### 1. 이해 
- 각 자릿수를 분리하는게 주요 문제일 듯 하다.
- 재귀를 이용하면 편할 것 같다.
- 0 또는 음수에 대해서도 처리한다.
- 주어진 정수를 10으로 나눈 나머지는 10^0 자릿수의 정수이다.
- 함수 하나의 크기를 5~8줄로 제한해본다.

#### 2. 계획
1. 주어진 정수(input)를 10으로 나눈 후 구해진 나머지(x)를 배열 A에 담는다.
2. input에서 1에서 구한 나머지를 빼고 10으로 나눈다.
3. 2의 결과를 input으로 하여 1을 반복한다.
4. 2의 결과가 0일 경우(input - x = 0) 더이상 계산할 자릿수가 없는 것이므로 종료한다.

#### 3. 실행

#### 4. 반성

### 문제2
주어진 문자열을 띄워쓰기 단위로 뒤집어서 출력한다.
ex) "I am a boy." -> "boy. a am I"

---

#### 1. 이해

#### 2. 계획

#### 3. 실행

#### 4. 반성
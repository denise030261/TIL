# 2026-10-27

## CS(컴퓨터 구조)

### 고급 언어와 저급 언어

#### 고급 언어

- 개발자가 이해하기 쉽게 만든 언어

- 예시) C++, C#, Python

#### 저급 언어

- 컴퓨터가 이해하고 실행하는 언어

- 예시) 기계어, 어셈블리어
  
  

#### 기계어

- 0과 1로 이루어진 명령어로 구성된 저급 언어

- 16진수로도 표현한다

#### 어셈블리어

- 0과 1로 이루어진 기계어를 읽기 편한 형태로 번역한 저급 언어

![f98af2d2-bf84-46d8-90cd-2761e38d76af](file:///C:/Users/admin/Pictures/Typedown/f98af2d2-bf84-46d8-90cd-2761e38d76af.png)



### 컴파일 언어와 인터프리트 언어

- 컴파일 언어
  
  - 컴파일 언어로 작성된 소스 코드는 컴파일러에 의해 저급 언어로 변환되고(이 과정을 컴파일이라고 한다) 컴파일 결과로 저급 언어인 목적 코드가 생성된다.
  - 소스 코드 컴파일 중 오류가 발생하면 소스 코드 전체가 실행되지 않음
  
  ![dcb22bb1-94db-40de-b8e1-bad32199691a](file:///C:/Users/admin/Pictures/Typedown/dcb22bb1-94db-40de-b8e1-bad32199691a.png)
  
  

  인터프리트 언어

* 인터프리터에 의해 한 줄씩 실행

* 소스 코드 전체가 저급 언어로 변환되기까지 기다릴 필요 없음

* 소스 코드 인터프리트 중 오류가 발생하면 오류 발생 전까지의 코드는 실행
  
  

![7d094b0c-0635-4837-a348-677c102207d8](file:///C:/Users/admin/Pictures/Typedown/7d094b0c-0635-4837-a348-677c102207d8.png)

-> 그렇다고 딱 잘라서 컴파일 언어, 인터프리터 언어로 나눌 수 없다. 둘 다 사용하는 언어도 있다



### 명령어의 구조

- 연산 코드와 오퍼랜드로 나누어짐

- 연산 코드는 수행할 연산, 오퍼랜드는 연산에 사용될 데이터 혹은 연산에 사용될 데이터가 저장된 위치를 저장한다
  
  - 연산에 사용될 데이터가 저장된 위치가 더 자주 저장된다.
  
  - 그래서 주소 필드라고 부르기도 한다

- 기계어, 어셈블리어도 명령어이다.
  
  

#### 오퍼랜드

- 오퍼랜드는 연산에 사용될 데이터 혹은 연산에 사용될 데이터가 저장된 위치를 저장한다
  
  - 연산에 사용될 데이터가 저장된 위치가 더 자주 저장된다.
  
  - 그래서 주소 필드라고 부르기도 한다

![2b37edd3-ebff-43a0-ad1c-ee7429218260](file:///C:/Users/admin/Pictures/Typedown/2b37edd3-ebff-43a0-ad1c-ee7429218260.png)



#### 연산 코드

- 연산에 사용될 데이터

- 종류
  
  - 데이터 전송
  
  - 산술/논리 연산
  
  - 제어 흐름 변경
  
  - 입출력 제어



#### 대표적인 연산 코드의 종류

- 데이터 전송
  
  - MOVE : 데이터를 옮겨라
  
  - STORE : 메모리에 저장하라
  
  - LOAD(FETCH) : 메모리에서 CPU로 데이터를 가져와라
  
  - PUSH : 스택에 데이터를 저장하라
  
  - POP : 스택의 최상단 데이터를 가져와라

- 산술/논리 연산
  
  - ADD/SUBTRACT/MULTIPLY/DIVIDE : 덧셈/뺼셈/곱셈/나눗셈을 수행하라
  
  - INCREMENT / DECREMENT : 오퍼랜드에 1을 더하라/오퍼랜드에 1을 빼라
  
  - AND/OR/NOT : AND/OR/NOT 연산을 수행하라
  
  - COMPARE : 두 개의 숫자 또는 TRUE/FALSE 값을 비교하라

- 제어 흐름 변경
  
  - JUMP : 특정 주소로 실행 순서를 옮겨라
  
  - CONDITIONAL JUMP : 조건에 부합할 때 특정 주소로 실행 순서를 옮겨라
  
  - HALT : 프로그램의 실행을 멈춰라
  
  - CALL : 되돌아올 주소를 저장한 채 특정 주소로 실행 순서를 옮겨라
  
  - RETURN : CALL을 호출할 때 저장했던 주소로 돌아가

- 입출력 제어
  
  - READ(INPUT) : 특정 입출력 장치로부터 데이터를 읽어라
  
  - WRITE(OUTPUT) : 특정 입출력 장치로 데이터를 써라
  
  - START IO : 입출력 장치를 시작하라
  
  - TEST IO : 입출력 장치의 상태를 확인하라



#### 명령어 주소 지정 방식

![4329f2c1-e6f9-4995-9041-0388229f67c9](file:///C:/Users/admin/Pictures/Typedown/4329f2c1-e6f9-4995-9041-0388229f67c9.png)

![2085622e-7a67-4356-bdd2-5585e26e8e7a](file:///C:/Users/admin/Pictures/Typedown/2085622e-7a67-4356-bdd2-5585e26e8e7a.png)

![76c6a40d-27c1-48b6-b146-82cf9cbc3478](file:///C:/Users/admin/Pictures/Typedown/76c6a40d-27c1-48b6-b146-82cf9cbc3478.png)

- 명령어에서 연산에 사용할 데이터가 아닌 주소를 가리키는 이유는 연산에 사용할 데이터의 양이 크지 않기 때문에 주소를 가리킨다



- 유효 주소(effective address)
  
  - 연산에 사용할 데이터가 저장된 위치

- 명령어 주소 지정 방식(addressing modes)
  
  - 연산에 사용할 데이터가 저장된 위치를 찾는 방법
  
  - 유효 주소를 찾는 방법
  
  - 다양한 명령어 주소 지정 방식들



- 즉시 주소 지정 방식(immediate addressing mode)
  
  - 연산에 사용할 데이터를 오퍼랜드 필드에 직접 명시
  
  - 가장 간단한 형태의 주소 지정 방식
  
  - 연산에 사용할 데이터의 크기가 작아질 수 있지만, 빠름

![d08a6f9d-616b-48c9-a37b-ffc60270c54f](file:///C:/Users/admin/Pictures/Typedown/d08a6f9d-616b-48c9-a37b-ffc60270c54f.png)



- 직접 주소 지정 방식(direct addressing mode)
  
  - 오퍼랜드 필드에 유효 주소 직접적으로 명시
  
  - 유효 주소를 표현할 수 있는 크기가 연산 코드만큼 줄어듦

![82fc2bd4-e6a0-46fe-be04-d0f92aba4943](file:///C:/Users/admin/Pictures/Typedown/82fc2bd4-e6a0-46fe-be04-d0f92aba4943.png)



- 간접 주소 지정 방식(indirect addressing mode)
  
  - 오퍼랜드 필드에 유효 주소의 주소를 명시
  
  - 앞선 주소 지정 방식들에 비해 속도가 느림

![40ceb60a-d5bc-4d18-b8f4-4c7cfee2e7b6](file:///C:/Users/admin/Pictures/Typedown/40ceb60a-d5bc-4d18-b8f4-4c7cfee2e7b6.png)



- 레지스터 주소 지정 방식(register addressing mode)
  
  - 연산에 사용할 데이터가 저장된 레지스터 명시
  
  - 메모리에 접근하는 속도보다 레지스터에 접근하는 것이 빠름

![1327ee71-a9c1-4be6-b10a-e25d7c9eb7ed](file:///C:/Users/admin/Pictures/Typedown/1327ee71-a9c1-4be6-b10a-e25d7c9eb7ed.png)

- 레지스터 간접 주소 지정 방식(register indirect addressing mode)
  
  - 연산에 사용할 데이터를 메모리에 저장
  
  - 그 주소를 저장한 레지스터를 오퍼랜드 필드에 명시

![c75ed155-4f85-4efa-a148-4b6793c589c8](file:///C:/Users/admin/Pictures/Typedown/c75ed155-4f85-4efa-a148-4b6793c589c8.png)



### C 언어 컴파일 과정

전처리 과정(preprocessing)

- 본격적으로 컴파일하기 전에 처리할 작업들

- 외부에 선언된 다양한 소스 코드, 라이브러리 포함 (e.g. #include)

- 프로그래밍의 편의를 위해 작성된 매크로 변환 (e.g. #define)

- 컴파일할 영역 명시 (e.g. #if, #ifdef)

컴파일 과정(compiling)

- 전처리가 완료 되어도 여전히 소스 코드

- 전처리 완료된 소스 코드를 저급 언어(어셈블리 언어)로 변환

어셈블 과정(assembling)

- 어셈블리어를 기계어로 변환

- 목적 코드(object file)를 포함하는 목적 파일이 됨

목적 파일 vs 실행 파일

- 목적 파일과 실행 파일은 둘 다 기계어로 이루어진 파일

- But, 목적 파일과 실행 파일은 다르다

- 목적 파일은 링킹(linking)을 거친 이후에야 실행 파일이 된다

![c0d9c206-b91c-4c7f-8fc3-21d33f044413](file:///C:/Users/admin/Pictures/Typedown/c0d9c206-b91c-4c7f-8fc3-21d33f044413.png)

![aa489489-4df2-4f39-a2b9-56dbf6c59b45](file:///C:/Users/admin/Pictures/Typedown/aa489489-4df2-4f39-a2b9-56dbf6c59b45.png)

링킹은 여러 개의 목적파일을 하나로 묶어 실행 파일로 만드는 과정이다.



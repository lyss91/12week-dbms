# 데이터베이스 모델링 및 ERD 및 MySQL 활용하기

- MySQL (DBMS 8.x)
  : RDBMS 를 다룬다. (Relation : 관계)

## 1. 요구사항 분석

- 회의 참석 (회의록)
- 회의록 검토 후 각 사항을 요구 사항 분서 (요구사항정의서, 업무지시서)

## 2. 요구사항 분석을 하는 이유

- 각 내용의 속성을 찾고, 분류
- 분류 된 내용을 모아서 Entity 를 생성한다.
- Entity 와 Entity 간의 관계를 찾는다.
- 요구사항 정의서 작성

### 2.1. 요구사항 분석 예

- 고객은 고객코드, 고객명, 전화번호, 이메일, 주소(기본주소 , 상세주소), 지역 , 가입일로 되어있다.
- 고객은 지역별로 관리되도록 한다.
- 지역은 지역코드와 지역명으로 되어 있고 지역명은 대한민국의 지역코드 (02:서울특별시)를 이용한다.
- 한 지역에는 여러 고객이 있을 수 있다.
- 제품은 제품코드 , 제품명 , 제품색상 , 가격으로 되어있다.
- 하나의 제품은 여러 색상을 가질 수가 있다.
- 고객은 등록된 제품을 구매 할 수 있다.
- 한 명의 고객은 여러 제품을 구매 할 수 있고 , 하 나의 제품은 여러 고객이 구매 할 수 있다.
- 고객이 제품을 구매 시 구매수량과 구매일자를 기록한다.

### 2.2. 요구사항 정의서 또는 업무 기술서 (회사마다 포맷이 다르다.)

![Image](https://github.com/user-attachments/assets/2487034b-ac24-4a7d-8311-560b661bbca3)

### 2.3. 속성(Arribute)을 찾기 후 Entity 정의하기

- 데이터 베이스 설계 전문가는 Entity 정의 후 속성을 선별해 나간다.
- 신입 데이터 설계자는 Arribute를 선별 후 Entity 를 정의함.

#### 2.3.1. 먼저 Entity 항목정리

: 명사소문자 추춴
![Image](https://github.com/user-attachments/assets/c436bc07-4d36-4ef0-95e8-003c8986e5e6)

#### 2.3.2. Entity 와 Entity 의 관계정리

: 동사소문자 추춴
![Image](https://github.com/user-attachments/assets/fbdd51a4-5598-4255-9eb5-bd692c4c7906)

## 3. ERD 그리기

### 3.1. 개념적 모델링

- Entity-Relationship Diagram
  ![Image](https://github.com/user-attachments/assets/8850d53f-139d-4b6f-aa56-f381c30aebc5)

### 3.2. 논리적 모델링

![Image](https://github.com/user-attachments/assets/b5610af3-1607-40ff-9d52-048dbf7c530a)

### 3.3. 물리적 모델링

- 고객 PK 후보
  ![Image](https://github.com/user-attachments/assets/c692dedf-40cd-4773-9d62-932b89df0736)

## 마일스톤

### STEP0. **github 마일스톤으로 진행상황 반영**
### STEP1. **프로젝트 설정 및 기본 구성**
- **1-1.**: 개발환경 준비
    - `의존성 설정` : Spring Data JPA, Spring Web, Lombok, MySQL, Spring Security 등/
    - `패키지 구조` : Layered Architecture Based + Clean


- **1-2.**: 데이터베이스 설정 (MySQL)
    - `application.yml`에 DB 설정 추가
    - DB 가라데이터 조회 테스트


- **1-3.**: 기본적인 엔티티 및 테이블 설계
    - `ERD` 설계 기반 JPA 엔티티 클래스 작성
    - 리포지토리 및 인터페이스 정의

---

### STEP2: **유저관련 API 구현**
- **2-1**: 잔액 충전 기능 구현
    - `POST /charge` 

  
- **2-2**: 잔액 조회 기능 구현
    - `GET /charge/{userId}`


- **2-3**: 단위 테스트 작성

  
- **2-4**: 코드 리팩토링 및 공통응답/예외 코드 추가 


---

### STEP3: **콘서트 관련 API 구현**
- **3-1**: 예약가능 콘서트 목록 조회 기능 구현
    - `GET /concert` 


- **3-2**: 콘서트 날짜 조회기반 좌석 수 기능 구현
  - `GET /concert/{date}`


- **3-3**: 콘서트 날짜 조회기반 좌석 리스트 기능 구현
  - `GET /concert/list/{date}`


- **3-4**: 단위 테스트 작성


- **3-5**: 코드 리팩토링 및 공통응답/예외 코드 추가


---


### STEP4: **예약 관련 API 구현**
- **4-1**: 예약 로직 구현
    - `POST /resreve`

- **4-2**: 단위 테스트 작성


- **4-3**: 코드 리팩토링 및 공통응답/예외 코드 추가


---


### STEP5: **결제 관련 API 구현**
- **5-1**: 결제 로직 구현
  - `POST /payment`

- **5-2**: 단위 테스트 작성


- **5-3**: 코드 리팩토링 및 공통응답/예외 코드 추가


---


### STEP6: **예약 + 결제 관련 API 구현**
- **6-1**: 통합 테스트 작성


- **6-2**: 동시성 로직 추가


- **6-3**: 동시성 통합 테스트 작성


---


### STEP7: **대기열 API 구현**
- **7-1**: 유저 대기열 토큰 발급 구현
  -  `POST /token`


- **7-2**: 예약 + 결제 로직에 대기열 관련 사전 로직 추가


- **7-3**: 테스트 

---


### STEP8: **대기열 고도화 및 부하테스트**
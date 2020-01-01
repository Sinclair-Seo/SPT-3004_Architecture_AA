# SPT-3004_Architecture_AA
조대협의 서버 사이드 대용량 아키텍처와 성능 튜닝

# Part_01 아키텍처 설계 방법
## [Chapter 01 소프트웨어 아키텍처의 설계](# Chapter 01 소프트웨어 아키텍처의 설계)

# Part_02 레퍼런스 아키텍처
## [Chapter 02 SOA](# Chapter 02 SOA)

## [Chapter 03 마이크로 서비스 아키텍처](# Chapter 03 마이크로 서비스 아키텍처)

## [Chapter 04 REST의 이해와 설계](# Chapter 04 REST의 이해와 설계)

## [Chapter 05 대용량 실시간 데이터 처리를 위한 람다 아키텍처](# Chapter 05 대용량 실시간 데이터 처리를 위한 람다 아키텍처)

# Part_04 대용량 아키텍처
## [Chapter 06 대용량 서비스 레퍼런스 아키텍처](# Chapter 06 대용량 서비스 레퍼런스 아키텍처)

## [Chapter 07 NoSQL](# Chapter 07 NoSQL)

# Part_04 성능 엔지니어링
## [Chapter 08 성능 엔지니어링의 정의와 범위](# Chapter 08 성능 엔지니어링의 정의와 범위)

## [Chaper 09 JVM과 톰캣 튜닝](# Chaper 09 JVM과 톰캣 튜닝)

## [Chapter 10 애플리케이션 서버의 병목 발견 방법](# Chapter 10 애플리케이션 서버의 병목 발견 방법)


# Chapter 01 소프트웨어 아키텍처의 설계
## 1. 아키텍처란 무엇인가?
[What is your definition of software
architecture?](https://resources.sei.cmu.edu/asset_files/FactSheet/2010_010_001_513810.pdf)

> "아키텍처는 비즈니스 요구 사항을 만족하는 시스템을 구축하기 위해서 전체 시스템에 대한 구조를 정의한 문서로, 시스템을 구성하는 컴포넌트와 그 컴포넌트 간의 관계, 그리고 컴포넌트가 다루는 정보(데이터)를 정의한다."

## 2. 아키텍처 설계 프로세스
- [Zachman Framework](https://en.wikipedia.org/wiki/Zachman_Framework)
- [TOGAF](https://www.opengroup.org/togaf) (The Open Group Architecture Framework)
- [Federal Enterprise Architecture](https://en.wikipedia.org/wiki/Federal_enterprise_architecture)

![아키텍처 설계 프로세스](/images/아키텍처_설계_프로세스.png "아키텍처 설계 프로세스")

## 3. 비즈니스 아키텍처 설계
### 3.1. 서비스 개요
### 3.2. 시장 현황 분석
[Gartner Magic Quadrant & Critical Capabilities](https://www.gartner.com/en/research/magic-quadrant)
### 3.3. 주요 기능 정의
### 3.4. 도메인 모델
### 3.5. 전체 아키텍처
### 3.6. 비즈니스 로드맵

## 4. 아키텍처 설계 원칙의 정의
## 5. 시스템 아키텍처 설계
![아키텍처 설계 프레임워크](/images/아키텍처_설계_프레임워크.png "아키텍처 설계 프레임워크")
### 5.1. 애플리케이션 아키텍처 설계
![애플리케이션 아키텍처 구성 요소](/images/애플리케이션_아키텍처_구성_요소.jpg "애플리케이션 아키텍처 구성 요소")

- 정적 아키텍처(Static Architecture)
    - 계층 모델    
    ![정적 아키텍처](/images/정적_아키텍처.png "정적 아키텍처")
    - 컴포넌트간 관계    
    ![컴포넌트 간 관계 표시도](/images/컴포넌트_간_관계_표시도.png "컴포넌트 간 관계 표시도")
    
- 동적 아키텍처(Dynamic Architecture)    
    ![동적 아키텍처 설계 예시](/images/동적_아키텍처_설계_예시.jpg "동적 아키텍처 설계 예시")
- 상세 아키텍처 설계 (Detail Architecture)    
    ![상세 아키텍처 예시](/images/상세_아키텍처_예시.png "상세 아키텍처 예시")
- 인터페이스 정의서(Interface Definition)
    - 프로토콜 정의 (REST, FTP, Google protocol buffer)
    - 메세지 포맷 정의 (REST API 정의서)
    
        [(참고)AWS S3 OpenAPI 명세서](https://docs.aws.amazon.com/AmazonS3/latest/API/archive-v2-RESTBucketGET.html)
    - 메세지 전달 방식 정의 (aka Message Exchange Pattern, MEP)
        - 동기/비동기
        - ETL 방식
    
    ![Rabbit MQ 기반의 메세지 패턴](/images/Rabbit_MQ_기반의_메세지_패턴.png "Rabbit MQ 기반의 메세지 패턴")
    
    [(참고)Enterprise Integration Patterns](https://en.wikipedia.org/wiki/Enterprise_Integration_Patterns)


### 5.2. 테크니컬 아키텍처
### 5.3. 데이터 아키텍처

## 6. 아키텍처 결정 프로세스
### 6.1. 아키텍처 결정 프로세스 정의
### 6.2. AD 템플릿

## 7. 효과적인 아키텍트의 역할과 종류
### 7.1. 아키텍트 역할
### 7.2. 아키텍트의 종류

## Chapter 02 SOA
### 1. SOA의 기본 개념
### 2. SOA에서 서비스의 정의
#### 2.1. 서비스의 구성
#### 2.2. 서비스의 특징
#### 2.3. 서비스의 종류

### 3. SOQ 아키텍처 모델
#### 3.1. Fundermental SOA
#### 3.2. Networked SOA
#### 3.3. Process Oriented SOA

### 4. SOA 아키텍처 모델의 구현
### 5. SOA 수행 방법론
#### 5.1. 기업의 전략
#### 5.2. 비용의 집행
#### 5.3. 제어와 통제
#### 5.4. 프로젝트 관리
#### 5.5. SOA 아키텍처 요약

## Part 03 마이크로 서비스 아키텍처
### 1. 모노리틱 아키텍처
#### 1.1. 문제점
### 2. 마이크로 서비스 아키텍처
#### 2.1. 아키텍처 구조
### 3. 마이크로 서비스 아키텍처의 문제점
#### 3.1. 성능
#### 3.2. 메모리
#### 3.3. 테스팅이 더 어려움
#### 3.4. 운영 관점의 문제
#### 3.5. 서비스 간 트랜잭션 처리
### 4. 거버넌스 모델
#### 4.1. Cross Functional Team
#### 4.2. You build, You run - DevOps
#### 4.3. Project vs. Product
#### 4.4. Self-organized Team
#### 4.5. Alignment
### 5. 진화형 모델(Evolutionery Model)
### 6. SOA와 비교

## Chapter 04 REST의 이해와 설계
### 1. REST의 기본
#### 1.1. HTTP 메서드
#### 1.2. REST의 리소스
#### 1.3. REST의 특성
#### 1.4. REST 안티 패턴
### 2. REST API 디자인 가이드
#### 2.1. REST URI는 단순하고 직관적으로 만들자
#### 2.2. 리소스 간의 관계를 표현하는 방법
#### 2.3. 에러 처리
#### 2.4. API 버전 관리
#### 2.5. 페이징
#### 2.6. 부분 응답 처리
#### 2.7. 검색(전역 검색과 지역 검색)
#### 2.8. HATEOS를 이용한 링크 처리
#### 2.9. 단일 API 엔드포인트 활용
### 3. REST의 문제점
### 4. REST API 보안
#### 4.1. REST API 보안 관점
#### 4.2. 인증
#### 4.3. 권한 인가
#### 4.4. 자바스크립트 클라이언트 지원

## Chapter 05 대용량 실시간 데이터 처리를 위한 람다 아키텍처
### 1. 람다 아키텍처란?
#### 1.1. 문제의 정의
#### 1.2. 배치 활용
#### 1.3. 실시간 집계 테이블 이용
### 2. 람다 아키텍처 활용
### 3. 람다 아키텍처 재구성
#### 3.1. RDBMS를 활용한 유연성 증대 방안
#### 3.2. 데이터 분석 도구를 이용한 새로운 분석 모델 개발

# Part_04 대용량 아키텍처
## Chapter 06 대용량 서비스 레퍼런스 아키텍처
### 1. 시스템 구조
### 2. Access Layer
#### 2.1. 웹 캐시
#### 2.2. Reverse Proxy
#### 2.3. API Gateway [선택 사항]
#### 2.4. 계정 관리
#### 2.5. 시스템 연동

### 3. Business Layer
#### 3.1. 동기 요청 처리
#### 3.2. 데이터 그리드를 이용한 상태 정보 저장소
#### 3.3. 메시지 큐를 이용한 비동기 요청 처리
#### 3.4. 임시 파일 작업 공간
#### 3.5. 메시징 프로토콜

### 4. Persistent Layer
#### 4.1. RDBMS
#### 4.2. 파일 시스템
#### 4.3. NoSQL

### 5. Analysis Layer
##### 5.1. 전통적인 OLAP 방식의 분석 시스템
##### 5.2. Map & Reduce 기반의 분석 시스템
##### 5.3. Map & Reduce + OLAP 형태의 데이터 분석 시스템
##### 5.4. 실시간 분석 시스템

### 6. OAM Layer
#### 6.1. CMDB (Configuration Management DB)
#### 6.2. 모니터링
#### 6.3. 로그 관리
#### 6.4. Configuration 관리

### 7. 클라우드 인프라
#### 7.1. 클라우드 컴퓨팅의 배포 모델에 따른 분류
#### 7.2. 클라우드 컴퓨팅의 서비스 단계에 따른 분류
#### 7.3. 클라우드 컴퓨팅의 장단점

### 8. 글로벌 서비스 아키텍처
#### 8.1. 법적인 이슈에 대한 검토
#### 8.2. 시스템 위치 선정
#### 8.3. 운영에 관련된 고려 사항
#### 8.4. 기술적인 고려 사항

## Chapter 07 NoSQL
### 1. NoSQL의 등장 배경
### 2. NoSQL의 특징
### 3. CAP 이론
### 4. NoSQL의 분류
#### 4.1. Key/Value Store
#### 4.2. Ordered Key/Value Store
#### 4.3. Document Key/Value Store

### 5. NoSQL 제퓸별 선호도
### 6. NoSQL과 기존 RDBMS와의 차이
### 7. NoSQL 사용 시 주의할 점
### 8. NoSQL 데이터 모델링
#### 8.1. NoSQL 디자인 패턴
#### 8.2. NoSQL과 RDBMS의 데이터 모델링 차이
#### 8.3. NoSQL 데이터 모델링 패턴
#### 8.4. NoSQL 데이터 모델링 절차

# Part_04 성능 엔지니어링
## Chapter 08 성능 엔지니어링의 정의와 범위
### 1. 성능 엔지니어링은 언제 해야 하는가?
### 2. 시스템 용량 산정
### 3. 성능 엔지니어링의 절차
#### 3.1. 목표와 모델의 정의
#### 3.2. 부하 생성
#### 3.3. 테스트와 모니터링
#### 3.4. 튜닝
#### 3.5. 반복

### 4. 성능 엔지니어링을 위해 필요한 것들

## Chaper 09 JVM과 톰캣 튜닝
### 1. JVM 튜닝
#### 1.1. GC란 무엇인가?
#### 1.2. GC의 동작방법은 어떻게 되는가?

### 2. 톰캣 튜닝
#### 2.1. 가정
#### 2.2. Listner 설정
#### 2.3. Connector 설정
#### 2.4. JVM 튜닝
#### 2.5. 메모리 옵션

## Chapter 10 애플리케이션 서버의 병목 발견 방법
### 1. Hang up과 Slow down 현상의 정의
### 2. 애플리케이션 서버와 User AP에서의 Slow down 분석
#### 2.1. 애플리케이션 서버의 기본 구조
#### 2.2. 스레드 덤프를 통한 애플리케이션 서버의 병목 구간 분석
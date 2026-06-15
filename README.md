# 안녕하세요! 저는 오영현입니다
 
<br/>
## 🚀 소개
 
요구사항이 바뀌어도 **코드 수정을 최소화하는 설계**를 가장 중요한 가치로 생각하는 개발자입니다.
 
- 🔭 Java/Spring 기반 백엔드 개발에 집중하고 있습니다
- 🌱 확장 가능한 백엔드 시스템과 직관적인 사용자 인터페이스 구축에 열정이 있습니다
- 💼 **300명이 실제로 사용하는 서비스**를 MVP부터 운영까지 직접 만들어본 경험이 있습니다
- 📫 언제나 협업과 새로운 기회에 열려있습니다!

<br/>

## 📝 자격증
![정보처리기사](https://img.shields.io/badge/정보처리기사-007396?style=for-the-badge&logo=java&logoColor=white)
![SQLD](https://img.shields.io/badge/SQLD-4479A1?style=for-the-badge&logo=mysql&logoColor=white)
![AI-POT%202급](https://img.shields.io/badge/AI--POT%20(프롬프트활용능력)%202급-8A2BE2?style=for-the-badge&logo=openai&logoColor=white)

<br/>

## 🛠️ 기술 스택

### 백엔드
![Java](https://img.shields.io/badge/Java-ED8B00?style=for-the-badge&logo=java&logoColor=white)
![Spring](https://img.shields.io/badge/Spring-6DB33F?style=for-the-badge&logo=spring&logoColor=white)
![Spring Boot](https://img.shields.io/badge/Spring_Boot-F2F4F9?style=for-the-badge&logo=spring-boot&logoColor=black)
![JPA](https://img.shields.io/badge/JPA-59666C?style=for-the-badge&logo=hibernate&logoColor=white)

### 프론트엔드
![React](https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB)
![TypeScript](https://img.shields.io/badge/TypeScript-007ACC?style=for-the-badge&logo=typescript&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)

### 데이터베이스 & 도구
![Oracle](https://img.shields.io/badge/Oracle-F80000?style=for-the-badge&logo=oracle&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL-00000F?style=for-the-badge&logo=mysql&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=for-the-badge&logo=postgresql&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-DC382D?style=for-the-badge&logo=redis&logoColor=white)

### 인프라 & 메시징
![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)
![Kafka](https://img.shields.io/badge/Apache_Kafka-231F20?style=for-the-badge&logo=apachekafka&logoColor=white)

<br/>

## 📊 GitHub 통계

<div align="center">

![Top Langs](https://github-readme-stats.vercel.app/api/top-langs/?username=dddd2356&layout=compact&theme=tokyonight&hide_border=true)

</div>

<br/>

## 🔥 연속 커밋

<div align="center">
  
![GitHub Streak](https://github-readme-streak-stats.herokuapp.com/?user=dddd2356&theme=tokyonight&hide_border=true)

</div>

<br/>

## 🧩 알고리즘
<div align="center">
  
[![Solved.ac Profile](http://mazassumnida.wtf/api/v2/generate_badge?boj=dddd2356)](https://solved.ac/dddd2356/)
![mazandi profile](http://mazandi.herokuapp.com/api?handle=dddd2356&theme=warm)
</div>

<br/>

## 🌟 주요 프로젝트
 
### 📦 [BoxOffice - MSA B2B 물류 허브 관리 플랫폼](https://github.com/boxoffice-sparta/boxoffice)
> 🏭 **Kafka 기반 이벤트 드리븐 MSA 물류 플랫폼**
- **개발 기간**: 2026.05 | **팀 구성**: 6인 | **담당**: 공통 모듈, 허브 서비스
- **기술 스택**: `Java` `Spring Boot` `Spring Security` `JPA` `Keycloak` `PostgreSQL` `Redis` `Kafka` `Docker` `Gemini AI` `Slack`
- **주요 기능 & 성과**:
  - 🔄 허브 폐쇄 시 **Drain 패턴(CLOSING→INACTIVE 2단계 삭제 정책)** 설계로 기존 배송 소진 후 안전 폐쇄하는 무중단 운영 흐름 구현
  - 📦 재고 이전 대상 선정 시 **FFD(First Fit Decreasing) 알고리즘**에 가용 용량·거리 복합 점수 정렬을 적용해 특정 허브 재고 집중 문제 해소
  - ⚡ 허브·경로 정보에 **Redis 캐싱(TTL 24h)** 적용 및 `@CacheEvict`로 수정·삭제 시 즉시 무효화하여 반복 DB 접근 제거
  - 📨 재고 이전 dispatch 후 `@TransactionalEventListener`로 Kafka 이벤트 발행, 배정 결과 Consumer 수신 → 실패 시 **1초 간격 3회 재시도 후 DLT 격리**로 메시지 유실 방지
  - 🧩 `ApiResponse` `PageResponse` `BaseException` `ErrorCode`를 **common 모듈**로 분리하여 전체 서비스에 일관된 API 규격 적용
### 🍱 [오늘 한끼 - 통합 배달 주문 관리 서비스](https://github.com/GolemOnce/Sparta-TodayEats)
> 🚀 **Gemini AI 연동 배달 주문·결제·내역 관리 플랫폼**
- **개발 기간**: 2026.04 | **팀 구성**: 5인 | **담당**: 주문 도메인
- **기술 스택**: `Java` `Spring Boot` `Spring Security` `JPA` `PostgreSQL` `Redis` `Docker` `AWS` `Gemini AI`
- **주요 기능 & 성과**:
  - 🔒 주문 상태 동시 변경 요청 시 낙관적 락(재시도 증가)·비관적 락(DB 블로킹) 대신 **WHERE절 현재 상태 조건부 UPDATE**로 전환해 DB 락 없이 동시성 제어
  - ⚛️ 취소 가능 여부 체크와 UPDATE 사이 타임갭으로 발생하는 레이스 컨디션을 **PostgreSQL Native Query 단일 쿼리**로 PENDING 조건과 상태 변경을 원자적으로 처리하여 조건 우회 가능성 제거
  - 🤖 상품 등록 시 Gemini AI가 상품 설명을 자동 생성하고 AI 요청·응답 이력을 별도 기록·관리
### 📋 [선한병원 전자결재 시스템](https://github.com/dddd2356/sunhan_electronic_payment_frontend)
> ⚡ **300명 실사용 기업용 전자결재 플랫폼**
- **개발 기간**: 2025.06 ~ 2026.03 | **팀 구성**: 1인 (풀스택)
- **기술 스택**: `Java` `Spring Boot` `Spring Security` `JPA` `MySQL` `Oracle` `React` `TypeScript`
- **주요 기능 & 성과**:
  - 📉 휴가 통계 조회 시 **N+1 문제(768개 쿼리)** 를 IN절 일괄 조회·Fetch Join·Map 인메모리 처리 조합으로 **6개 쿼리로 통합, 응답 속도 3s → 0.7s (77% 개선)**
  - 🔐 배포 후 쿠키 미전달 인증 오류 → LocalStorage 긴급 복구 후 **httpOnly 쿠키 방식으로 전면 리팩토링**하여 XSS 취약점 해소
  - 🗃️ 내부망 Oracle 종속 문제를 **MySQL 마이그레이션 및 외부망 전용 인증 시스템 구축**으로 서비스 접근성·운영 연속성 확보
  - 📄 `@TransactionalEventListener(AFTER_COMMIT)`으로 트랜잭션 확정 후에만 **PDF 아카이빙** 실행하여 결재 문서 원본 무결성 확보
  - ⚙️ **동적 결재선 구조** 구현으로 조직 구조 변경 시 코드 수정·재배포 없이 즉시 대응 가능
### 🏥 [선한병원 건강정보고속도로](https://github.com/dddd2356/sunhan_myhealthway_frontend)
> 🔐 **암호화 기반 안전한 의료 정보 웹뷰어 연결 플랫폼**
- **개발 기간**: 2025.08 | **팀 구성**: 1인 (풀스택)
- **기술 스택**: `Spring Boot` `Spring Security` `JPA` `MySQL` `React` `TypeScript`
- **주요 기능 & 성과**:
  - 🔒 C# 환경 암호화 미동작 문제를 **Spring 기반 공통 암호화 API**로 해결하여 플랫폼 간 암호화 호환성 확보
  - 🌐 암호화된 URL 기반 외부 EHR 뷰어 안전 연결로 의료 정보 보안 표준 준수

<div align="center">
 
### 🚧 **현재 집중 분야**
**🔥 확장 가능한 백엔드 시스템 & 직관적인 사용자 인터페이스** | `Spring Boot` `React` `TypeScript`
 
</div>

## 📈 활동 그래프

<div align="center">
  
![dddd2356's github activity graph](https://github-readme-activity-graph.vercel.app/graph?username=dddd2356&theme=tokyo-night&hide_border=true)

</div>

<br/>

## 💻 개발 환경

```javascript
const dddd2356 = {
    code: ["Java", "TypeScript", "SQL"],
    askMeAbout: ["백엔드 설계", "MSA", "성능 최적화", "데이터베이스 설계"],
    technologies: {
        backend: ["Spring Boot", "Spring Security", "JPA"],
        frontend: ["React", "TypeScript", "CSS"],
        database: ["MySQL", "PostgreSQL", "Redis", "Oracle"],
        messaging: ["Kafka"],
        infra: ["Docker", "AWS"],
        tools: ["IntelliJ IDEA"]
    },
    currentFocus: "MSA 환경에서의 확장 가능한 백엔드 시스템 설계"
};
```

<br/>

## 🤝 연락하기
<div align="center">
  
[![Email](https://img.shields.io/badge/Email-dudgus2109%40gmail.com-red?style=for-the-badge&logo=gmail&logoColor=white)](mailto:dudgus2109@gmail.com)
[![GitHub](https://img.shields.io/badge/GitHub-dddd2356-black?style=for-the-badge&logo=github&logoColor=white)](https://github.com/dddd2356)

[![Profile Views](https://komarev.com/ghpvc/?username=dddd2356&color=blueviolet&style=for-the-badge&label=VISITORS)](https://github.com/dddd2356)

</div>

---

<div align="center">
  
*"좋은 코드는 그 자체로 최고의 문서이다." - Steve McConnell*

⭐️ From [dddd2356](https://github.com/dddd2356)

</div>

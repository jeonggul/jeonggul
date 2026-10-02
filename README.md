# 이정하 | Java 백엔드 개발자 포트폴리오

Java와 Spring Boot로 웹 서비스를 개발했습니다. 개인 프로젝트에서는 매매 기록과 손익 계산, 실시간 시세 연동을 구현하고 AWS에 배포했습니다. 팀 프로젝트에서는 회원 인증과 세션 관리, 영화 예매 기능을 담당했습니다.

[GitHub](https://github.com/jeonggul)

## 대표 프로젝트

### 01. MIJANG

**미국 주식 매매 기록과 투자 회고 서비스**  
2026.08–2026.09 · 개인 프로젝트

매매 당시의 판단을 기록하고, 보유 자산과 주가·환율 손익을 확인하는 서비스입니다. 기획부터 구현, 테스트, 배포까지 수행했습니다.

- 과거 거래 변경 시 시간순으로 보유 수량을 재계산하고 초과 매도를 검증했습니다.
- 거래 변경과 재계산을 하나의 트랜잭션으로 처리했습니다.
- WebSocket으로 수신한 시세를 SSE로 전달하고, 여러 사용자의 중복 종목 구독을 관리했습니다.

**사용 기술:** Java 17, Spring Boot, MyBatis, MySQL, Thymeleaf, JavaScript, AWS EC2

[상세 포트폴리오](https://github.com/jeonggul/jeonggul/blob/main/projects/mijang/README.md) · [소스 코드](https://github.com/jeonggul/mijang)

### 02. Knowva

**코딩 입문자를 위한 웹 학습 플랫폼**  
2026.06.17–2026.07.27 · 7인 팀 프로젝트

웰컴 튜토리얼부터 회원가입·로그인, 비밀번호 재설정까지 구현하고 인증·보안·세션 관리를 담당했습니다.

- 소셜 인증과 회원 생성을 분리해 추가 정보 입력 중 이탈한 사용자의 불완전한 계정이 남지 않도록 했습니다.
- 비밀번호 변경 이후에는 기존 자동 로그인 쿠키로 세션을 복원할 수 없도록 했습니다.
- 재설정 토큰의 사용 처리와 비밀번호 변경을 하나의 트랜잭션으로 묶었습니다.

**사용 기술:** Java 17, Spring Boot, Spring MVC, MyBatis, MySQL, HttpSession, OAuth, JUnit

[상세 포트폴리오](https://github.com/jeonggul/jeonggul/blob/main/projects/knowva/README.md) · [팀 저장소](https://github.com/hyunkyumlee/Acorn-E-Learning)

### 03. POPFLIX

**영화 예매 및 리뷰 서비스**  
2026.04.29–2026.05.14 · 5인 팀 프로젝트

조장으로 참여해 영화관·상영관과 좌석 선택, 예매 등록·조회·변경·취소를 구현했습니다. 공통 화면 통합과 병합 충돌 정리에도 참여했습니다.

- 예매와 좌석 데이터를 하나의 DB 연결과 트랜잭션으로 처리했습니다.
- 좌석 변경과 취소 시 관련 데이터를 함께 갱신하도록 구성했습니다.
- 로그인한 사용자의 예매인지 확인한 뒤 변경·취소를 처리했습니다.

**사용 기술:** Java, Servlet, JSP, JDBC, Oracle, HTML, CSS, JavaScript

[상세 포트폴리오](https://github.com/jeonggul/jeonggul/blob/main/projects/popflix/README.md) · [팀 저장소](https://github.com/Rustapex/JavaServletMVC-Project)

## 기술과 사용 경험

| 기술 | 직접 사용한 경험 |
| --- | --- |
| Java | 거래 수량·손익 계산, 인증 로직, 예매 처리 |
| Spring Boot / Spring MVC | 웹 요청 처리, 서비스 계층, 인터셉터 기반 인증 |
| MyBatis / JDBC | 데이터 조회·변경과 트랜잭션 처리 |
| MySQL / Oracle | 계정·거래·예매 데이터 저장과 연관 데이터 관리 |
| JUnit | 계산 로직, 거래 수정, 인증 서비스·인터셉터 테스트 |
| AWS EC2 / Nginx | MIJANG 배포, HTTPS 구성, 배포 환경 오류 수정 |

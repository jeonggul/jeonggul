<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&amp;color=0%3AF3F6FA%2C100%3ADCE5F1&amp;height=210&amp;section=header&amp;text=JEONGHA+LEE&amp;fontColor=142D50&amp;fontSize=48&amp;fontAlignY=38&amp;desc=JAVA+BACKEND+DEVELOPER&amp;descSize=17&amp;descAlignY=60&amp;animation=fadeIn" width="100%" alt="JEONGHA LEE — Java Backend Developer" />

# 안녕하세요, 개발자 이정하입니다

<img src="https://readme-typing-svg.demolab.com?font=Fira+Code&amp;size=20&amp;duration=3000&amp;pause=1400&amp;color=315B88&amp;center=true&amp;vCenter=true&amp;width=700&amp;height=52&amp;lines=Java+%2B+Spring+Boot%3BFrom+transaction+logic+to+deployment" alt="Java와 Spring Boot를 사용하는 백엔드 개발자" />

거래 기록의 정확성과 사용자 인증 흐름을 고민하며 웹 서비스를 개발했습니다.<br/>
개인 프로젝트의 기획·배포와 팀 프로젝트의 인증·예매 기능 구현을 경험했습니다.

<br/>

<img src="https://img.shields.io/badge/Java-142D50?style=for-the-badge" alt="Java" />
<img src="https://img.shields.io/badge/Spring%20Boot-142D50?style=for-the-badge&amp;logo=springboot&amp;logoColor=white" alt="Spring Boot" />
<img src="https://img.shields.io/badge/MyBatis-142D50?style=for-the-badge" alt="MyBatis" />
<img src="https://img.shields.io/badge/MySQL-142D50?style=for-the-badge&amp;logo=mysql&amp;logoColor=white" alt="MySQL" />
<img src="https://img.shields.io/badge/JUnit5-142D50?style=for-the-badge&amp;logo=junit5&amp;logoColor=white" alt="JUnit5" />
<img src="https://img.shields.io/badge/Git-142D50?style=for-the-badge&amp;logo=git&amp;logoColor=white" alt="Git" />
<img src="https://img.shields.io/badge/AWS%20EC2-142D50?style=for-the-badge" alt="AWS EC2" />
<img src="https://img.shields.io/badge/Nginx-142D50?style=for-the-badge&amp;logo=nginx&amp;logoColor=white" alt="Nginx" />

<br/><br/>

<a href="https://github.com/jeonggul/jeonggul#대표-프로젝트">대표 프로젝트</a> · <a href="https://github.com/jeonggul/jeonggul#기술과-사용-경험">기술과 사용 경험</a>

</div>

<br/>

## 대표 프로젝트

### 01. MIJANG

<p align="center"><img src="https://raw.githubusercontent.com/jeonggul/jeonggul/main/assets/mijang-dashboard.png" width="760" alt="MIJANG 서비스 화면" /></p>

<sub>화면 금액은 시연 데이터입니다.</sub>

**미국 주식 매매 기록과 투자 회고 서비스**  
2026.08–2026.09 · 개인 프로젝트

매매 당시의 판단을 기록하고, 보유 자산과 주가·환율 손익을 확인하는 서비스입니다. 기획부터 구현, 테스트, 배포까지 수행했습니다.

- 과거 거래 변경 시 시간순으로 보유 수량을 재계산하고 초과 매도를 검증했습니다.
- 거래 변경과 재계산을 하나의 트랜잭션으로 처리했습니다.
- WebSocket으로 수신한 시세를 SSE로 전달하고, 여러 사용자의 중복 종목 구독을 관리했습니다.

**사용 기술:** Java 17, Spring Boot, MyBatis, MySQL, Thymeleaf, JavaScript, AWS EC2

[상세 포트폴리오](https://github.com/jeonggul/jeonggul/blob/main/projects/mijang/README.md) · [소스 코드](https://github.com/jeonggul/mijang)

<br/>

---

### 02. Knowva

<p align="center"><img src="https://raw.githubusercontent.com/jeonggul/jeonggul/main/assets/knowva-login.png" width="580" alt="Knowva 서비스 화면" /></p>

**코딩 입문자를 위한 웹 학습 플랫폼**  
2026.06.17–2026.07.27 · 7인 팀 프로젝트

웰컴 튜토리얼부터 회원가입·로그인, 비밀번호 재설정까지 구현하고 인증·보안·세션 관리를 담당했습니다.

- 소셜 인증과 회원 생성을 분리해 추가 정보 입력 중 이탈한 사용자의 불완전한 계정이 남지 않도록 했습니다.
- 비밀번호 변경 이후에는 기존 자동 로그인 쿠키로 세션을 복원할 수 없도록 했습니다.
- 재설정 토큰의 사용 처리와 비밀번호 변경을 하나의 트랜잭션으로 묶었습니다.

**사용 기술:** Java 17, Spring Boot, Spring MVC, MyBatis, MySQL, HttpSession, OAuth, JUnit

[상세 포트폴리오](https://github.com/jeonggul/jeonggul/blob/main/projects/knowva/README.md) · [팀 저장소](https://github.com/hyunkyumlee/Acorn-E-Learning)

<br/>

---

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

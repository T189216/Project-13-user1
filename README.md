# 예시어플 백엔드 서버 개발


## 📙 프로젝트 개요

### 프로젝트 설명

우리의 과외 매칭 플랫폼은 누구나 선생님이 되어 지식을 나누고, 누구나 학생이 되어 새로운 분야를 배울 수 있는 열린 교육 커뮤니티를 제공합니다. 어떤 분야에서든 자신의 전문 지식을 공유하고 가르칠 수 있는 선생님들과 그 지식을 습득하고 싶은 학생들이 모두 자유롭게 참여할 수 있습니다. 우리의 플랫폼은 교육의 경계를 허물어 사용자들에게 더 많은 학습 기회를 제공하며, 학습과 가르침의 자유로운 교류를 촉진합니다.

 **배경**

- 자기 재능을 누구나 수업하고 원하는 분야를 배울 수 있는 서비스
    - Java Spring을 사용하여 웹사이트를 구축하는 것이 목표인 백엔드 프로젝트
- client 간에 매칭으로 웹사이트 내에서 결제 API를 통한 결제 관리
    - 토스페이먼츠, 카카오페이 비즈니스, 아임포트(포트원)으로 결제
- SpringBoot, H2, JPA 등을 사용한 규격을 이용한 백엔드 구현
- 웹사이트 배포 목적

### 💻 담당 업무

**SpringBoot Backend 개발**

- 담당 인원 : 각 파트 별 2인 (회원,게시판,결제)
- Spring API
    - Spring: `SpringBoot2.6.4`, `Gradle`, `Java21`, `lombok`
    - Security: `security`
    - DB: `Mybatis`, `Jpa`
    - API Document: `springdoc-openapi-ui(Swagger)`
    
- Database: `MySQL`
- dev Tool: `HeidiSQL DataGrip`, `putty winscp`, `Postman Swagger-UI`

## 팀 구성원, 개인 별 역할

---

프로젝트 팀 구성원을 기재해 주시고, 그 주의 팀원이 어떤 역할을 맡아서 개발을 진행했는지 구체적으로 작성해 주세요. 🙂

- 해당 역할을 그대로 따를 필요는 없습니다!

## 팀 내부 회의 진행 회차 및 일자

---

예) 1회차(2024.01.10) 구글 밋 진행, (OOO님 불참)

- 일주일 간 진행한 내부 회의 횟수와 일자, 진행 방법, 불참 인원을 위와 같이 작성해 주세요.

## 현재까지 개발 과정 요약 (최소 500자 이상)

---

현재까지 진행하고 있는 개발 현황을 기능별 목표, 목표달성률, 성과자체평가(상세히) 작성해주세요.

- 성과자체평가는 ‘기술적으로 새로 알게된 점, 어려웠던 점, 아쉬운 점, 시도해볼 점' 등을 작성해 주시면 됩니다 🙂
- 팀원 각자 현재 구현하고 있는 것을 적어주세요. :)
- ex) 기능별 목표: 암기장 삭제하기 기능 추가 / 목표달성률: 50% - 마켓에서 등록해제는 가능, 내 암기장 삭제는 아직 미구현 / 지속적으로 수정사항이 발생하여 완성도를 올리는 중, 현재 관련 문서 참고 중

## 🛠 프로젝트 상세 정보

### 🎆 서비스 아키텍처

해당 문서에서는 아래 그림의 `SpringBoot` 에 대해 다룹니다.


### 🤔 주요 기능

- 회원가입 / 로그인: 게시글을 작성하고, 원하는 게시글에 댓글을 작성할 수 있습니다.
- 게시글 작성: **개인정보** (ex: 연락처), **활동 분야(카테고리),** 제공할 수 있는 서비스, 구체적으로 어떤 서비스를 진행할지를 작성할 수 있습니다. **※ 보라색 글씨는 필수로 작성합니다.**
    - 게시글 수정/삭제: 내가 작성한 게시글을 수정하거나 삭제할 수 있습니다.
- 댓글 작성: 원하는 상품이 있는 게시글에 댓글을 작성할 수 있습니다.
    - 댓글 수정/삭제: 내가 작성한 댓글을 수정하거나 삭제할 수 있습니다.
- 게시글 리스트: 제공하는 서비스가 작성된 게시글들을 조회할 수 있습니다.
- 마이페이지: 내 정보를 조회할 수 있습니다.
    - 회원정보 수정: 내 정보(ex: 프로필, 연락처)를 수정할 수 있습니다.
    - 회원탈퇴: 플랫폼에서 모든 개인 정보가 삭제됩니다.
    - 내가 쓴 글: 내가 쓴 글들을 조회할 수 있습니다.
    - 내가 쓴 댓글: 내가 쓴 댓글들을 조회할 수 있습니다.
    - 결제내역: 내가 결제한 상품들의 결제내역을 확인할 수 있습니다.
- 장바구니: 원하는 서비스를 결제하기 위해 원하는 상품을 저장하고 관리할 수 있습니다.
- 결제: 원하는 서비스를 제공받기 위해 결제를 할 수 있습니다.


## 개발 과정에서 나왔던 질문 (최소 200자 이상)

---

개발을 진행하며 나왔던 질문 중 핵심적인 것을 요약하여 작성해 주세요 🙂

- 질의응답 과정 중 해결되지 않은 질문을 정리하여도 좋습니다.

## 개발 결과물 공유

---

Github Repository URL:

- 필수) 팀원들과 함께 찍은 인증샷(온라인 만남시 스크린 캡쳐)도 함께 업로드 해주세요 🙂

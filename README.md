🚀 React & Spring Boot Member Management (CRUD)
이 프로젝트는 Spring Boot JPA와 React를 결합하여 기본적인 회원 관리 시스템(CRUD)을 구현한 예제 학습 프로젝트입니다. 코드 아키텍처의 발전 단계에 따라 3개의 프로젝트로 구성되어 있습니다.

📂 프로젝트 구성 (Project Structure)
폴더명	기술 스택	주요 특징
jpa3	Spring Boot, JPA, MySQL	백엔드 Restful API 서버 구현 중심
prjJpa	React, Axios, Bootstrap	프론트엔드 구현 (Axios 통신 로직이 각 컴포넌트에 분산)
prjJpaAxios	React, Axios Service Layer	[최적화] Axios 통신 부분을 memberService.js로 모듈화
✨ 주요 기능 (Key Features)
👤 회원 등록: 모달 창을 통한 신규 회원 추가
📋 목록 조회: 페이징 처리된 회원 리스트 출력
✏️ 정보 수정: 기존 회원 데이터 불러오기 및 수정 기능
🗑️ 회원 삭제: 선택한 회원 정보 삭제 (Confirm 알림 포함)
⚡ API 최적화: Axios 인터셉터 및 서비스 레이어 분리를 통한 유지보수성 향상
🛠 Tech Stack
Backend
   

Frontend
  

🚀 실행 방법 (Getting Started)
1. Backend (jpa3)
src/main/resources/application.yml 설정 확인
./gradlew bootRun 실행 (포트: 8080)
2. Frontend (prjJpaAxios)
cd prjJpaAxios
npm install
npm run dev (포트: 5173)
💡 학습 포인트
Dirty Checking: JPA 변경 감지를 이용한 효율적인 Update 처리
DTO Transfer: Entity와 DTO 간의 역할 분리 및 변환 로직
Service Layer Pattern: React에서 API 호출 로직을 한곳으로 모아 유지보수성을 극대화하는 패턴 학습

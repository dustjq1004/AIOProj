# AIO - Olive Bro

### 스프링 프로젝트 - ERP 관리자 시스템
<p align="center">
<kbd>
<img width="1368" style="border: 20px solid black;" alt="image" src="https://github.com/dustjq1004/AIOProj/assets/73459956/f60ea66f-942b-491d-bb98-326e1b0668a7">
</kbd>
<kbd>
<img width="1184" style="border: 20px solid black;" alt="image" src="https://github.com/dustjq1004/AIOProj/assets/73459956/8540b643-70dc-4143-9ce6-e9019107b058">
</kbd>
</p>

### 프로젝트 소개

All In One 프로젝트는 급증하는 드럭스토어의 인기로 인한 재고, 거래처, 재무 관리의 어려움을 해결하고자 만든 ERP 프로그램입니다. 화장품 관련되는 프로그램을 제작하기 위하여 화장품 관련해서 조사해보았을 때 줄어드는 로드 샵에 반면에 급증하는 드럭 스토어로 인해 거래처 관리, 물품관리, 재무 관리에 대해서 어렵고 복잡하다는 것을 알게 됐습니다. 그래서 ERP 시스템을 도입하여 데이터 중복을 제거하고 단일 데이터로 부서에서 데이터를 입력하면 전 부서가 필요에 따라 정보를 활용할 수 있고 재고관리와 다양한 업무처리의 효율을 증진시킬 수 있도록 프로그램을 개발했습니다.

### 1. 프로젝트 설명

학원 과정은 Spring Freamework 학습하는 것이었습니다. 하지만 더 나아가 Spring Boot, Spring security, Spring Jpa를 학습하게 되면 프로젝트를 신속하고 효율적이게 구현할 수 있다는 것을 알게 됐습니다. 3개의 모듈은 학습하기가 어렵다는 단점이 있지만, Spring Framework 기반 웹 프로젝트를 구현할 때 많은 이점을 주는 강력한 도구입니다. 그렇기 때문에 ERP 프로그램을 만들기 위해서 앞서 언급된 Spring Boot, Security, Jpa를 사용하여 개발했습니다.

- 스프링부트 웹 기반 ERP 프로그램 개발
-   기간 : 2020-12-04 ~ 2021-01-04 (4주)
-   팀 인원 : 4명
-   개발환경, 사용 기술
    -   IDE : Intelij 2020-03
    -   View : JSP, CSS, JavaScript, Jquery, Ajax, thymeleaf
    -   Back : Java 1.8, Spring Boot, Spring Jpa, Spring Security, Oracle DB
    -   Tools, Api : Maven, Github, GooleDrive, OvenApp.io, Draw.io, Powerpoint 2016, Github DeskTop, npm, Google mail Api, Daum 주소 검색 Api

### 2. AIO - ERP 관리자 
    
-   프로젝트 기여도 : 20%
-   역할 : Front & Backend 개발
-   담당 기능
    -   로그인 기능
    -   Spring Security 권한 부여 기능
        - 권한없는 사용자 페이지 접근시 에러페이지 처리
        - 퇴사자 로그인 거부 처리
    -   인사기능
        - CRUD
        - 이미지 data uri 사용
        - 구글 메일 api 사용
        - 다음 주소 검색 api 사용
    -   메인페이지
        - 출퇴근 기능
        - openweathermap.js 사용
    -   마이페이지
        - 회원 정보 수정
        - 근태 기록
          - fullCalendar.js 사용

### 3. 개발 관련 설명

스프링이 제공해주는 강력한 기능들을 적극 활용한 프로젝트라고 할 수 있습니다. 제가 담당한 부분은 로그인과 인사관련 기능이기 때문에 Spring Security를 중점으로 개발했고, 다른 팀원들은 Jpa를 적극 활용하여 개발 속도를 높일 수 있었습니다. 또한 단위 테스트 코드를 작성하진 않았지만 더미 데이터 담당, 개발 DB 구축 등 업무를 분담하여 효율성을 높였고, 테스트를 수월하게 할 수 있는 환경을 제공했습니다.

Spring Security를 사용하여 인사에 대한 권한을 업무에 따라 나누어 페이지마다 접근 권한을 설정하여 보안을 한층 높였습니다. 그리고 스프링 내부에 정적 팩토리 메서드로 구현되어있는 `PasswordEncoderFactories.createDelegatingPasswordEncoder()` 를 사용해 Bctypt 해시 함수를 사용해서 민감한 정보를 암호화 했습니다.

<p align="center">
<img width="32%" alt="image" src="https://github.com/dustjq1004/AIOProj/assets/73459956/18715337-55b2-44d3-9272-f3e7552394d6">
<img width="30%" alt="image" src="https://github.com/dustjq1004/AIOProj/assets/73459956/90219544-6d88-4bfa-bf88-b0fd6882dd7f">
<img width="29.5%" alt="image" src="https://github.com/dustjq1004/AIOProj/assets/73459956/6e41498c-10ab-4885-95d7-78bb0feb31a0">
</p>

그 외에 부가적인 기능으로는 Spring Interceptor를 이용하여 출퇴근 기록과 퇴근 후에는 당일에 다시 출근할 수 없도록 로직을 처리하고, 사원 검색에서 현재 출근 중인 사람을 확인할 수 있습니다. 또한 프로필 사진 등록과 인사 권한이 있는 사람만 비밀번호 초기화 기능을 사용할 수 있도록 개발했습니다.

### 4. Entity Relationship Diagram (ERD)

<img width="1698" alt="image" src="https://github.com/dustjq1004/AIOProj/assets/73459956/1b409290-ba15-4596-8fab-2ea255b24f70">

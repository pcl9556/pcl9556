
# 👩🏻‍💻 안녕하세요, 웹 개발자 박채린입니다.

Java & Spring Boot 기반 백엔드와  
React 기반 프론트엔드를 함께 다루는 웹 개발자입니다.  
사용자 경험과 서비스 운영 편의성을 모두 고려한 웹 서비스를 만드는 데 관심이 많습니다.

## 🚀 Tech Stack

**Backend**
- Java 17, Spring Boot, Spring Security, JWT
- MyBatis
- REST API 설계
<p>
  <img src="https://img.shields.io/badge/Java-007396?style=for-the-badge&logo=openjdk&logoColor=white"/>
  <img src="https://img.shields.io/badge/SpringBoot-6DB33F?style=for-the-badge&logo=springboot&logoColor=white"/>
  <img src="https://img.shields.io/badge/SpringSecurity-6DB33F?style=for-the-badge&logo=springsecurity&logoColor=white"/>
  <img src="https://img.shields.io/badge/MyBatis-000000?style=for-the-badge&logo=mybatis&logoColor=white"/>
</p>

**Frontend**
- JavaScript(ES6+), React, Vite
- React Router, Axios
- HTML5, CSS3
<p>
  <img src="https://img.shields.io/badge/React-61DAFB?style=for-the-badge&logo=react&logoColor=black"/>
  <img src="https://img.shields.io/badge/Vite-646CFF?style=for-the-badge&logo=vite&logoColor=white"/>
  <img src="https://img.shields.io/badge/JavaScript-ES6+-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black"/>
  <img src="https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white"/>
</p>

**Database & Infra**
- MySQL, MySQL Workbench
- Git / GitHub, SourceTree
- Docker, AWS
- Figma, Notion
<p>
  <img src="https://img.shields.io/badge/MySQL-4479A1?style=for-the-badge&logo=mysql&logoColor=white"/>
  <img src="https://img.shields.io/badge/MySQLWorkbench-006EAB?style=for-the-badge&logo=mysql&logoColor=white"/>
  <img src="https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white"/>
  <img src="https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white"/>
  <img src="https://img.shields.io/badge/SourceTree-0052CC?style=for-the-badge&logo=sourcetree&logoColor=white"/>
  <img src="https://img.shields.io/badge/Swagger-85EA2D?style=for-the-badge&logo=swagger&logoColor=black"/>
  <img src="https://img.shields.io/badge/Postman-FF6C37?style=for-the-badge&logo=postman&logoColor=white"/>
  <img src="https://img.shields.io/badge/Figma-F24E1E?style=for-the-badge&logo=figma&logoColor=white"/>
  <img src="https://img.shields.io/badge/Notion-000000?style=for-the-badge&logo=notion&logoColor=white"/>
</p>

## ⭐️ Projects

### 1. POPPOP – 팝업스토어 예약 & 운영 관리 서비스 (Team Project)
> 팝업스토어를 운영하는 **매니저**를 위한 예약·운영 관리 웹 서비스
> > 팀 프로젝트 (2025)

#### ✔ Manager 기능 전담 개발자 
- `/manager/mypopup`  
  - 팝업 등록/조회/상세/수정 화면 개발  
  - 예약 현황 페이지 + 페이지네이션 + 검색/필터  
- `/manager/dashboard`  
  - KPI(예약 수/사용자 행동 유형 비율 등) + Recharts 기반 시각화  
  - 차트 데이터 전처리 및 상태 관리 설계
- `/manager/reservation`  
  - 예약 리스트
  - csv, print 기능
- React + Spring Boot API 연동 (상태 관리, 에러 처리, 인증 흐름 대응)
  - 예약 목록 UI/UX 개선 (페이지네이션, 검색 필터, 반응형 구조)

 #### ✔ 데이터 모델링 & DB 설계 (DBA Support)
- MySQL **스키마 설계·제약조건·인덱스 구성 논의 및 설계**
  - `member`, `popup_store`, `reservation`, `review` 등 핵심 테이블 구조 설계에 참여  
  - 외래키, UNIQUE, ENUM-like 구조, ON UPDATE CASCADE 등 실제 운영 기준으로 제약조건 설계  
  - 성능을 고려한 인덱스 구성 (`idx_member_role`, `idx_popup_store_category` 등)
 
#### ✔ **서비스 브랜딩 & 시각 자료 제작**
- POPPOP Manager 페이지 디자인  
- POPPOP 포스터/브랜딩 자료 제작 (서비스 톤·매너 통일)
- 색상·타이포·브랜딩 가이드 통일

### ‼️ 트러블슈팅

- **JWT 인증 및 권한 기반 보호 API 처리**
  - 직접 JWT를 개발하진 않았지만, 매니저 페이지 개발 과정에서 발생한 401/403 오류를 분석하고  
    Axios 인터셉터 & ProtectedRoute 패턴으로 인증 흐름을 안정화했습니다.

- **MyBatis 매핑 오류 및 SQLSyntaxErrorException 해결**
  - 컬럼명 불일치, ResultMap 매핑 오류, DTO 필드 누락으로 발생하는 쿼리 오류를 디버깅하며  
    Mapper–DTO–DB 구조 전반을 깊이 이해하게 되었습니다.

- **React 비동기 상태 문제 해결**
  - useEffect 의존성 누락으로 API가 중복 호출되는 문제, 페이지네이션 시 state와 요청 값이 불일치하는 문제를 해결하며  
    React 렌더링 사이클과 비동기 상태 처리 방식을 정확히 이해하게 되었습니다.

- **대용량 예약 데이터 로딩 시 UI 성능 저하 문제 해결**
  - 예약 데이터가 많아질수록 DOM 렌더링 비용 증가로 화면 버벅임이 발생했습니다.  
    key 안정화, 불필요 렌더 제거, 리스트 구조 최적화 등을 적용해 성능을 개선했고  
    데이터 증가 상황에서도 안정적인 화면 성능을 유지할 수 있었습니다.

- **예약 목록 UI 레이아웃 깨짐 문제 해결**
  - flex 기반 카드 레이아웃이 데이터 증가 시 부모 컨테이너 밖으로 튀어나오거나 간격이 불규칙해지는 문제가 발생했습니다.  
    grid 기반으로 구조를 재설계하고, margin 대신 gap을 사용해 간격을 통일했으며  
    overflow 제어를 통해 레이아웃 안정성을 확보했습니다.
 

## 📍  Links
  - GitHub Repo: (나중에 POPPOP 레포 링크 추가)
  - 프로젝트 상세 설명(노션): 추가예정!

## ✏️ Learning & 관심사

- Spring Security / JWT 구조 /httpOnly Cookie 더 깊게 이해하기
- 대시보드·통계 페이지처럼 데이터를 시각화하는 UI 만들기
- 협업 가능한 코드 구조와 Git 브랜치 전략 익히기


## 📫 Contact

- Email: pcl9556@naver.com
- GitHub: https://github.com/pcl9556
- Notion Portfolio: 추가예정!

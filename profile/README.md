# 💜 취향 가득, 팝업스토어 모음 플랫폼 'PORONG'

> **경험 중심 소비 트렌드로 급부상한 팝업스토어!**  
> 파편화된 정보를 한곳에 모으고, 실시간 혼잡도 공유와 게이미피케이션 요소를 결합한  
팝업스토어 통합 플랫폼 포롱(PORONG)입니다.

<img width="1920" height="910" alt="image" src="https://github.com/user-attachments/assets/e236bd4a-46a3-4993-8cef-eef8142eda4c" />

<br>

## 👥 팀원 소개 및 역할 분배
전 팀원이 프론트엔드와 백엔드를 완전 담당하여 기능을 완성했습니다.

| **이주현 (팀장)** | **고유정** | **서지현** |
| :---: | :---: | :---: |
| 메인 페이지, 찾기 페이지 | 팝업 상세, 후기, 마이페이지 | 로그인/회원가입, 관리자 페이지 |
| 메인/검색/필터 API, 최근 리뷰 API | 리뷰 CRUD, 도감/예약 CRUD API | 회원 CRUD, 팝업 CRUD, 통계 집계 API |

| 이주현 | 고유정 | 서지현 |
|:------:|:------:|:------:|
| <img src="https://github.com/hana03030.png" width="100%"/> | <img src="https://github.com/daenggg.png" width="100%"/> | <img src="https://github.com/jhwest-dev.png" width="100%"/> | 
| [@hana03030](https://github.com/hana03030) | [@daenggg](https://github.com/daenggg) | [@jhwest-dev](https://github.com/jhwest-dev) |

<br>

## 📌 기획 배경 및 해결책
- **Pain Point:** SNS에 흩어진 정보 탐색의 어려움, 방문 전 현장 혼잡도 파악 불가능으로 인한 시간 낭비
- **Our Solution:** 
  1. **통합 정보 제공:** 흩어진 팝업 정보를 한곳에서 스마트하게 탐색 및 필터링
  2. **사용자 참여형 데이터:** 유저들의 실제 후기를 기반으로 한 실시간 평균 혼잡도 공유
  3. **게이미피케이션:** 리뷰 작성 시 귀여운 키링 수집 유도로 유저 활동성 촉진

<br>

## 🛠️ 시스템 아키텍처 & 페이지 구조
### [ 시스템 구조 ]
- **Frontend:** HTML5, CSS3, JavaScript (kakaomap API 연동)
- **Backend:** Spring Boot, MySQL
<img width="2346" height="1660" alt="image" src="https://github.com/user-attachments/assets/e5021d21-6bb1-4050-9bf4-893576b78c6b" />


### [ 서비스 Flow ]
- **구매자(User):** 홈(랭킹) ➡️ 찾기(필터링) ➡️ 팝업 상세(예약/리뷰) ➡️ 마이페이지(키링 도감)
- **판매자(Admin):** 팝업 관리 ➡️ 팝업 등록(자동 좌표 변환) ➡️ 예약/후기 확인 및 통계 대시보드
<img width="1777" height="800" alt="image" src="https://github.com/user-attachments/assets/f7e16871-232b-4071-abf8-e153babe8c4c" />


<br>

## 🔗 레포지토리 바로가기
- 💻 [Po-Rong-Frontend](https://github.com/Po-Rong/Po-Rong-Frontend) - UI 컴포넌트, 가로 스크롤 및 배너 애니메이션 구현
- ⚙️ [Po-Rong-Backend](https://github.com/Po-Rong/Po-Rong-Backend) - 자동 위경도 변환, 혼잡도 통계 산출 로직 및 API 서버

# 💜 팝업스토어 모음 플랫폼 PORONG
> 파편화된 정보를 한곳에 모으고, 실시간 혼잡도 공유와 게이미피케이션 요소를 결합한  
팝업스토어 통합 플랫폼 포롱(PORONG)입니다.

<img width="1920" height="910" alt="image" src="https://github.com/user-attachments/assets/e236bd4a-46a3-4993-8cef-eef8142eda4c" />

---

## 👥 팀원 소개 및 역할 분배

전 팀원이 프론트엔드와 백엔드를 담당하여 기능을 완성했습니다.

| 이주현 | 고유정 | 서지현 |
|:------:|:------:|:------:|
| <img src="https://github.com/hana03030.png" width="100%"/> | <img src="https://github.com/daenggg.png" width="100%"/> | <img src="https://github.com/jhwest-dev.png" width="100%"/> | 
| [@hana03030](https://github.com/hana03030) | [@daenggg](https://github.com/daenggg) | [@jhwest-dev](https://github.com/jhwest-dev) |
| 메인 페이지, 찾기 페이지 | 팝업 상세, 후기, 마이페이지 | 로그인/회원가입, 관리자 페이지 |
| 찜/리뷰 CRUD, 최근 리뷰 API | 도감/예약 CRUD, 혼잡도 API | 회원/팝업 CRUD, 통계 집계 API |

---

## 📌 기획 배경 및 해결책

- **Pain Point:** SNS에 흩어진 정보 탐색의 어려움, 방문 전 현장 혼잡도 파악 불가능으로 인한 시간 낭비
- **Our Solution:** 
  1. **통합 정보 제공:** 흩어진 팝업 정보를 한곳에서 스마트하게 탐색 및 필터링
  2. **사용자 참여형 데이터:** 유저들의 실제 후기를 기반으로 한 실시간 평균 혼잡도 공유
  3. **게이미피케이션:** 리뷰 작성 시 귀여운 키링 수집 유도로 유저 활동성 촉진

---

## 🌟 핵심 기능 (Core Features)

| 01. 실시간 인기도 및 랭킹 시스템 | 02. 조건별 팝업 필터링 |
| :---: | :---: |
| <img width="2560" height="1389" alt="image" src="https://github.com/user-attachments/assets/cc199119-c781-449f-8462-eb5b82d2e4d3" /> | <img width="2560" height="1399" alt="image" src="https://github.com/user-attachments/assets/93a5c194-d688-4a34-9223-44cef35e1a14" /> |
| 실시간 찜 수 데이터를 분석하여 1~10위 인기 팝업을 집계하고, 금/은/동 왕관 및 NEW 뱃지를 시각화하여 트렌드를 한눈에 제공합니다. | 카테고리, 지역, 운영 상태 결합 필터링과 Kakao Map API를 연동하여 내 주변 팝업 위치를 직관적으로 탐색합니다. |
| **03. 실시간 별점 & 혼잡도 리뷰** | **04. 키링 도감** |
| <img width="2560" height="1313" alt="image" src="https://github.com/user-attachments/assets/7b9cc55b-a6da-43d8-9f11-bbdd5b4fd460" /> | <img width="2560" height="1270" alt="image" src="https://github.com/user-attachments/assets/38b97823-6229-4f19-ae40-4713b1563656" /> |
| 이미지 바이너리 파일과 폼 데이터를 동시에 패킹하여 전송하며, 별점 및 3단계 현장 혼잡도 게이지 인터랙션을 지원합니다. | 리뷰 작성을 통해 수집한 산리오 키링을 마이페이지에서 확인하고, 미획득 아이템은 그림자 처리하여 수집 욕구를 자극합니다. |
| **05. 실시간 예약 및 후기 모니터링** | **06. 자동 좌표 변환 팝업 등록** |
| <img width="2560" height="1304" alt="image" src="https://github.com/user-attachments/assets/c39bdc23-a579-4dc6-bf2d-872ba37af2a3" /> | <img width="2560" height="1185" alt="image" src="https://github.com/user-attachments/assets/14485c36-1707-4959-8d46-ef8bb3b08a1c" /> |
| 일자별/회차별 타임테이블에 따른 실시간 예약 현황을 파악하고, 유저들이 남긴 생생한 현장 혼잡도 후기를 한눈에 모니터링합니다. | 신규 팝업스토어 등록 시, 입력한 주소 데이터를 기반으로 위경도 좌표를 자동 변환하여 Kakao Map API에 실시간 마커로 연동합니다. |

---

## 🛠️ 시스템 아키텍처 & 페이지 구조
### [ 시스템 구조 ]

- **Frontend:** HTML5, CSS3, JavaScript (kakaomap API 연동)
- **Backend:** Spring Boot, MySQL

<img width="2346" height="1660" alt="image" src="https://github.com/user-attachments/assets/e5021d21-6bb1-4050-9bf4-893576b78c6b" />

### [ 서비스 Flow ]

- **구매자(User):** 홈(랭킹) ➡️ 찾기(필터링) ➡️ 팝업 상세(예약/리뷰) ➡️ 마이페이지(키링 도감)
- **판매자(Admin):** 팝업 관리 ➡️ 팝업 등록(자동 좌표 변환) ➡️ 예약/후기 확인 및 통계 대시보드

<img width="1777" height="800" alt="image" src="https://github.com/user-attachments/assets/f7e16871-232b-4071-abf8-e153babe8c4c" />

---

## 🔗 레포지토리 바로가기
- 💻 [Po-Rong-Frontend](https://github.com/Po-Rong/Po-Rong-Frontend) - UI 컴포넌트, 가로 스크롤 및 배너 애니메이션 구현
- ⚙️ [Po-Rong-Backend](https://github.com/Po-Rong/Po-Rong-Backend) - 자동 위경도 변환, 혼잡도 통계 산출 로직 및 API 서버

<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:FFD1A9,50:FFB6B9,100:FFC6E0&height=160&section=header&text=D-Order%20V3&fontSize=50&fontColor=ffffff"/>

### 🍻 University Festival Booth Management Platform
동국대학교 축제 주점 통합 운영 플랫폼

<img src="https://img.shields.io/badge/Django-092E20?style=for-the-badge&logo=django&logoColor=white"/>
<img src="https://img.shields.io/badge/Spring Boot-6DB33F?style=for-the-badge&logo=springboot&logoColor=white"/>
<img src="https://img.shields.io/badge/PostgreSQL-4169E1?style=for-the-badge&logo=postgresql&logoColor=white"/>
<img src="https://img.shields.io/badge/Redis-DC382D?style=for-the-badge&logo=redis&logoColor=white"/>

</div>

<br>

## 📖 Overview

D-Order는 대학 축제 기간 동안 발생하는 주문, 결제, 재고 및 주점 운영을 디지털화하기 위해 개발한 통합 운영 플랫폼입니다.
V3에서는 실제 운영 경험을 바탕으로 시스템을 전면 개선하고, **Spring Boot 서버와 Django 서버를 Redis로 연동**하여 서비스를 확장했습니다.

<br>

## 📊 Results

| Metric | Result |
| :--- | ---: |
| 🍺 Booths | **23** |
| 👥 Users | **2,500+** |
| 📈 Page Views | **130,000+** |
| ⚡ Events | **220,000+** |
| 💰 Operating Profit | **233,000원** |

<br>

## 🛠 Tech Stack

**Backend**
- Python, Django, Django REST Framework
- Java, Spring Boot

**Database**
- PostgreSQL, Redis

**Analytics**
- Google Analytics 4

**Collaboration**
- Git, GitHub, Notion, Slack

<br>

## ✨ Main Features

- QR 기반 주문 시스템
- 실시간 주문 및 결제 관리
- 관리자(Admin) 시스템
- 파트너센터 운영
- 현장 서버 화면
- 운영자 권한 관리
- 주문 통계
- Google Analytics 연동

<br>

## 👨‍💻 My Role — 박선우 (Django Backend)

- **메뉴 / 주문 도메인** Django 백엔드 개발
- **Redis를 활용한 Django ↔ Spring Boot 서버 간 통신** 구현
- Google Analytics 데이터 분석
- 운영 현장 대응, 카카오톡 1:1 문의 대응

<br>

## 🚀 What Changed from V2?

✅ Spring Boot 연동 (Redis 기반 서버 간 통신)
✅ Google Analytics 적용
✅ 서버 화면 추가
✅ 운영 파트너센터 구축
✅ 현장 대응 프로세스 구축
✅ 사용자 피드백 기반 개선

<br>

## 📈 Google Analytics

- 총 조회수 **130,734**
- 총 이벤트 **221,136**
- 활성 사용자 **2,500+**

<br>

<br>

## 🔗 Website
https://2602-d-order-home-page.vercel.app

<br>

---

## 👥 V3 Contributors

| 이름 | Email | 담당 |
| --- | --- | --- |
| 강근우 | gn00py48@dgu.ac.kr | Spring Boot |
| 오태준 | xownswns@naver.com | Spring Boot |
| 이동건 | plasma1233@dgu.ac.kr | Infra / Spring Boot |
| 임수빈 | forestbin0420@dgu.ac.kr | Django |
| **박선우** | sunwoo030616@dgu.ac.kr | **Django** |
| 차은호 | eunho2002@dgu.ac.kr | Infra / Django |

<br>

## 📁 프로젝트 구조

```
2026-d-order-backend-v3/
├── .env                          # 환경 변수 (Django + Docker) notion 참조
├── README.md                     # 이 파일
├── docker-compose.local.yml      # 로컬 개발 환경시 postgre + redis 컨테이너 만들기
├── docker-compose.prod.yml       # 작성 예정 / 배포 시 docker-compose
├── docker-compose.staging.yml    # 작성 예정 / 개발서버 docker-compose
├── django/
│   ├── manage.py
│   ├── requirements.txt          # Python 의존성 파일들
│   ├── apps/
│   └── project/                  # Django 프로젝트 폴더
└── Spring/                       # Spring
```

<br>

## 📝 커밋 및 PR 컨벤션

시간이 없기 때문에.. 최소한의 태그만 사용하는 것으로 컨벤션 정했습니다.

### ✅ Commit Convention

| 태그 | 설명 | 예시 |
| --- | --- | --- |
| Feat | 새로운 기능 추가(새 API/유스케이스/도메인 기능) | `Feat: 주문 생성 API 추가` |
| Fix | 버그 수정(오류/예외/로직 결함) | `Fix: 결제 승인 시 NPE 수정` |
| Design | UI 스타일 및 레이아웃 변경(백엔드엔 보통 거의 없음; Swagger/문서 UI 정도만 해당) | `Design: Swagger UI 테마 변경` |
| Docs | 문서 수정(README, API 문서, 주석 등) | `Docs: 로컬 실행 방법 업데이트` |
| Refactor | 리팩토링(기능 변화 없음, 구조/가독성/중복 개선) | `Refactor: 주문 서비스 메서드 분리` |
| Chore | 설정/패키지/환경 변경(빌드, 의존성, 설정 파일 등) | `Chore: Spring profile 설정 정리` |

> ⚠️ Feat은 진짜 "새 기능"에만! 오타 수정 등에는 Fix 사용

- **Refactor**: 기존 코드의 내부 구조를 개선하는 데 중점을 둠. 외부 동작은 동일하지만 코드를 더 효율적이고 읽기 쉽게 만드는 변경에 해당 (예: 함수 분리, 변수명 개선, 중복 코드 제거).
- **Chore**: 프로젝트의 빌드 환경, 종속성, 관리 관련 작업에 중점을 둠. 코드 자체의 로직 변경보다는 개발 환경 설정, 라이브러리 업데이트, 빌드 스크립트 수정 등.

### ✅ PR 제목 규칙

| 아이콘 | 태그 | 설명 | 예시 |
| --- | --- | --- | --- |
| ✨ | [Feature] | 새로운 기능 추가 | ✨ [Feature] #12 - 마이페이지 기능 추가 |
| 🐛 | [Fix] | 버그 수정 | 🐛 [Fix] #15 - 로그인 버튼 오류 수정 |
| 🎨 | [Design] | UI 스타일 및 레이아웃 | 🎨 [Design] #21 - 헤더 스타일 변경 |
| 📝 | [Docs] | 문서 수정 | 📝 [Docs] #30 - README 사용법 수정 |
| ♻️ | [Refactor] | 리팩토링 | ♻️ [Refactor] #35 - API 요청 함수 리팩토링 |
| 🔧 | [Chore] | 환경 설정 변경 | 🔧 [Chore] #40 - webpack 설정 변경 |

<br>

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:FFC6E0,50:FFB6B9,100:FFD1A9&height=100&section=footer"/>

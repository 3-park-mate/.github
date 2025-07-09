# 🚗 ParkMate - 주차장 중개 플랫폼

ParkMate는 운전자에게 실시간 주차 공간 정보를 제공하고, 주차장 소유주에게는 유휴 공간을 효과적으로 활용할 수 있는 기회를 제공하는 MSA(Microservice Architecture) 기반 주차장 중개 플랫폼입니다.

## 🏛️ 시스템 아키텍처

본 프로젝트는 각 기능이 독립적인 마이크로서비스로 분리되어 있으며, API Gateway를 통해 외부 요청을 처리합니다. 서비스 간의 통신, 서비스 검색 및 관리를 위해 Service Discovery, Message Queue 등의 패턴을 적용했습니다.

<img src="./images/시스템아키텍처.png">

## CI/CD 파이프라인

## 🧾 ERD

<img src="./images/erd.png">

## ✨ 주요 기능

- **사용자**: 회원가입, 로그인, 프로필 관리
- **호스트**: 주차장 등록, 관리 및 수익 정산
- **주차장 검색**: 위치 기반 실시간 주차장 정보 조회, 필터링 및 검색
- **예약 및 결제**: 간편한 주차 공간 예약 및 결제 시스템
- **알림**: 예약, 결제 등 주요 이벤트에 대한 실시간 알림
- **이용 내역**: 사용자의 주차 이용 내역 조회

## 🛠️ 기술 스택

| 구분 | 기술 |
| --- | --- |
| **Backend** | Java, Spring Boot, Spring Cloud, JPA, QueryDSL |
| **Frontend** | Next.js, TypeScript, TurboRepo |
| **Database** | MySQL, MongoDB, Redis |
| **Infrastructure** | AWS, Docker, GIthub Actions, Kafka, Nginx |
| **API Gateway** | Spring Cloud Gateway |
| **Service Discovery**| Netflix Eureka |
| **Build Tool** | Gradle |
| **Common** | RESTful API, OAuth 2.0  |

## 🚀 마이크로서비스 목록

각 서비스에 대한 자세한 내용은 해당 디렉토리의 `README.md` 파일을 참고해주세요.

| Service | Repository | Description |
| --- | --- | --- |
| **Frontend** | [`FE-park-mate`](https://github.com/3-park-mate/FE-park-mate) | 사용자 및 호스트를 위한 웹 애플리케이션 |
| **Discovery Server** | [`parkmate-discovery-server`](https://github.com/3-park-mate/parkmate-discovery-server/) | 서비스 등록 및 검색을 담당하는 Eureka 서버 |
| **API Gateway** | [`parkmate-gateway-service`](https://github.com/3-park-mate/parkmate-gateway-service/) | 모든 클라이언트 요청의 단일 진입점 |
| **Auth Service** | [`parkmate-auth-service`](https://github.com/3-park-mate/parkmate-auth-service/) | 주차장 소유주(호스트) 관련 기능 관리 |
| **User Service** | [`parkmate-user-service`](https://github.com/3-park-mate/parkmate-user-service/) | 사용자 인증 및 회원 정보 관리 |
| **Host Service** | [`parkmate-host-service`](https://github.com/3-park-mate/parkmate-host-service) | 주차장 소유주(호스트) 관련 기능 관리 |
| **Parking Service** | [`parkmate-parking-service`](https://github.com/3-park-mate/parkmate-parking-service) | 주차장 정보(CRUD) 관리 (Write Model) |
| **Parking Read Service** | [`parkmate-parking-read-service`](https://github.com/3-park-mate/parkmate-parking-read-service) | 주차장 정보(READ) 관리 (READ Model) |
| **Batch Service** | [`parkmate-batch-service`](https://github.com/3-park-mate/parkmate-batch-service) | 배치 관련 기능 관리 |
| **Review Service** | [`parkmate-review-service`](https://github.com/3-park-mate/parkmate-review-service) | 주차장 리뷰 관련 기능 관리 |
| **Review Read Service**| [`parkmate-review-read-service`](https://github.com/3-park-mate/parkmate-review-read-service)| 리뷰 READ 데이터 관리 |
| **Reservation Service**| [`parkmate-reservation-service`](https://github.com/3-park-mate/parkmate-reservation-service)| 주차장 예약 관리 |
| **Order Service** | [`parkmate-order-service`](https://github.com/3-park-mate/parkmate-order-service) | 예약에 따른 주문 생성 및 관리 |
| **Payment Service** | [`parkmate-payment-service`](https://github.com/3-park-mate/parkmate-payment-service) | 결제 처리 및 외부 PG 연동 |
| **Notification Service**| [`parkmate-notification-service`](https://github.com/3-park-mate/parkmate-notification-service)| 푸시 알림 발송 |
| **History Service** | [`parkmate-user-parking-history`](https://github.com/3-park-mate/parkmate-user-parking-history)| 주차장 입/출차 내역 관리 |
| **Chat Service** | [`parkmate-chat-service`](https://github.com/3-park-mate/parkmate-chat-service) | 채팅 관련 기능 관리 |

## 📱 화면 구성

|  로그인   |  메인   |
| :---: | :---: |
| <img src="https://github.com/user-attachments/assets/533f07fa-223e-4dad-ad09-3f1a1a2fd51c" width="300"/>    |  <img src="./시스템아키텍처.png" width="300"/>   |   

## 이벤트 스토밍
<img src="./images/이벤트스토밍.png">

## 🔧 Git
### 이슈
### 커밋
### PR

## 🗓️ 일정 관리
### WBS

## 📑 API 명세서

## 👥 팀원 소개
| 이름 | 역할 |
| --- | --- |
| 정영록 | BE(팀장), 주차장, 예약, 주문, 알림 도메인 |
| 송민석 | BE, INFRA |
| 김보미 | BE |
| 윤예지 | FE |
| 윤채영 | FE |


## 💬 느낀점
| 이름 | 느낀점 |
| --- | --- |
| 정영록 | - |
| 송민석 | - |
| 김보미 | - |
| 윤예지 | - |
| 윤채영 | - |

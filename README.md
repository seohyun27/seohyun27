<div align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=0:FF9EB1,50:B39CD0,100:98D6EA&height=250&section=header&text=Hello,%20I'm%20Seohyun!&fontColor=ffffff" alt="header">

  <h3>🚀 Thinking & Documenting Backend Developer</h3>
  <p>
    <b>"이유 없는 코드는 없다"</b><br>
    기능 구현을 넘어 <b>탄탄한 설계</b>와 <b>명확한 문서화</b>를 지향하는 백엔드 개발자입니다.<br>
    팀의 성장을 돕는 <b>적극적인 소통</b>과 <b>지식 공유</b>를 즐깁니다.
  </p>
</div>

<br/>

## 🛠 Tech Stack

**Main Stack (Backend)**
<br>
<img src="https://img.shields.io/badge/Java-007396?style=for-the-badge&logo=java&logoColor=white"/>
<img src="https://img.shields.io/badge/Spring_Boot-6DB33F?style=for-the-badge&logo=spring-boot&logoColor=white"/>
<img src="https://img.shields.io/badge/JPA-6DB33F?style=for-the-badge&logo=hibernate&logoColor=white"/>
<img src="https://img.shields.io/badge/MySQL-4479A1?style=for-the-badge&logo=mysql&logoColor=white"/>

**Sub & Tools**
<br>
<img src="https://img.shields.io/badge/Kotlin-7F52FF?style=for-the-badge&logo=kotlin&logoColor=white"/>
<img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white"/>
<img src="https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white"/>
<img src="https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white"/>

<br/>

## 🏆 Featured Projects
> **혼자보다 함께할 때 더 멀리 간다.**<br>
> 팀의 목표를 최우선으로 적극적인 리딩과 원활한 소통을 통해 완성해 온 프로젝트들입니다.

### 🎵 Humix — AI 허밍 작곡 서비스
**Main API Server Owner (Backend)**
<br>
<img src="https://img.shields.io/badge/Java-007396?style=flat-square&logo=java&logoColor=white"/>
<img src="https://img.shields.io/badge/Spring_Boot-6DB33F?style=flat-square&logo=spring-boot&logoColor=white"/>
<img src="https://img.shields.io/badge/MariaDB-003545?style=flat-square&logo=mariadb&logoColor=white"/>
<img src="https://img.shields.io/badge/AWS_EC2-232F3E?style=flat-square&logo=amazon-aws&logoColor=white"/>
<img src="https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white"/>

사용자의 허밍을 AI로 편곡·완성곡화하는 서비스의 **메인 비즈니스 로직 및 데이터 흐름을 총괄하는 API 서버**입니다. 클라이언트 요청을 처리하고, 무거운 AI 음악 생성 작업을 독립된 워커 노드로 안전하게 위임·동기화합니다.

- **3-Tier + MSA 워커 분리**: 고부하 AI 모델 구동 환경을 메인 서버에서 분리, 비동기 Job Queue 기반 마이크로서비스로 구축
- **비동기 처리 파이프라인**: S3 업로드 → Job 등록 → SSE 기반 실시간 진행률 전송 → Webhook 콜백으로 상태 동기화
- **비용 최적화 아키텍처 설계**: GPU 상시 구동 대신 RunPod Serverless + Job Queue 체계 채택, ARM64(t4g.small) 인스턴스에 Spring Boot·Nginx·MariaDB·Librosa를 컨테이너로 격리 구동해 **월 운영비 2만원 이하** 유지

🔗 GitHub: [바로가기](https://github.com/Humix-Project/humix-backend)

<br/>

### 🎪 WagleWagle — 실시간 축제 혼잡도 모니터링
**Backend Developer & DevOps** *(2026.03~2026.05)*
<br>
<img src="https://img.shields.io/badge/Spring_Boot-6DB33F?style=flat-square&logo=spring-boot&logoColor=white"/>
<img src="https://img.shields.io/badge/Redis-DC382D?style=flat-square&logo=redis&logoColor=white"/>
<img src="https://img.shields.io/badge/MySQL-4479A1?style=flat-square&logo=mysql&logoColor=white"/>
<img src="https://img.shields.io/badge/Uber_H3-000000?style=flat-square&logo=uber&logoColor=white"/>
<img src="https://img.shields.io/badge/NCP-03C75A?style=flat-square"/>
<img src="https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white"/>

야외 축제장의 **실시간 인파 혼잡도**를 집계해 히트맵으로 제공하는 위치 기반 서비스입니다. 수천 명 동시 접속 환경의 트래픽 처리가 핵심 과제였습니다.

- **Redis Geo 기반 위치 처리**: 초당 갱신되는 위치 데이터를 RDB 대신 In-Memory Geo 구조로 처리해 `O(1)~O(logN)`으로 최적화, Expire 기반 Heartbeat 미응답자 자동 제외
- **Uber H3 공간 집계**: 좌표를 육각형 그리드로 사전 집계해 프론트엔드 전송량 90% 이상 절감
- **NCP 기반 인프라 설계**: VPC로 DB/스토리지는 Private Subnet, API·Redis는 Public Subnet에 분리해 최소 권한 원칙 기반 네트워크 설계

🔗 GitHub: [바로가기](https://github.com/wagle-project/wagle-server)

<br/>

### 📚 API Wiki — API 선택 가이드 플랫폼
**Tech Leader & DevOps** *(2026.01 ~ 2026.02)*
<br>
<img src="https://img.shields.io/badge/Spring_Boot-6DB33F?style=flat-square&logo=spring-boot&logoColor=white"/>
<img src="https://img.shields.io/badge/MySQL-4479A1?style=flat-square&logo=mysql&logoColor=white"/>
<img src="https://img.shields.io/badge/AWS_EC2-232F3E?style=flat-square&logo=amazon-aws&logoColor=white"/>
<img src="https://img.shields.io/badge/GitHub_Actions-2088FF?style=flat-square&logo=github-actions&logoColor=white"/>
<img src="https://img.shields.io/badge/Nginx-009639?style=flat-square&logo=nginx&logoColor=white"/>

개발자들이 실사용 경험을 공유하며 API를 선택할 수 있도록 돕는 커뮤니티 위키 서비스입니다. 다양한 직군과 협업하며 **테크 리더**로서 설계와 배포 전 과정을 조율했습니다.

- **배포 안정성 확보**: 쉘 스크립트(`nohup`) 한계를 극복하고 Systemd 도입, 비정상 종료 시 자동 복구 환경 구축
- **환경별 보안 설정 분리**: `@ConditionalOnProperty`로 로컬(H2)/운영(RDS) 보안 설정을 단일 코드베이스에서 유연하게 격리
- **데이터 파이프라인 자동화**: 기획 데이터를 Python으로 전처리해 DB 맞춤형 포맷으로 마이그레이션
- **버그 수정 사례**: API 상세 조회 시 조회수 미증가 문제를, `@Transactional` 오버라이딩과 JPA Dirty Checking으로 해결
- **코드 리뷰를 통한 N+1 문제 개선**: PR 리뷰 중 리스트 순회 시 발생하는 N+1 쿼리를 직접 발견, IN 절 기반 배치 조회로 개선하는 방향을 코드와 함께 제시

🔗 GitHub: [바로가기](https://github.com/umc-apiwiki/APIWIKI_BE_v1)

<br/>

<details>
<summary><h2>💡 Engineering Foundation (펼쳐보기)</h2></summary>

> **프레임워크 없이 구조의 필요성을 깨닫다.**<br>
> 웹 개발 학습 전, 순수 Java Swing으로 구현하며 MVC 패턴과 Client-Server 구조를 독자적으로 도출해낸 프로젝트입니다.

**[Customer Tracking System](https://github.com/seohyun27/customer-tracking.git)** *(Java Swing, Simulated Server)*

- **MVC 패턴의 발견**: 코드 복잡도 해결을 위해 `MainControl`(Router), `View`, `Domain`으로 역할 분리
- **Client-Server 구조 설계**: 데이터 중앙 관리의 필요성을 느껴 로컬 환경 내 가상 서버(`Server.java`) 구현
- **데이터 설계**: `String`↔`int` 변환 클래스를 설계해 DB 인덱싱과 유사한 데이터 최적화 경험
- **결과**: [시연 영상 보기](https://youtu.be/kMNQep4sots)

</details>

<br/>

## 📚 Study & Knowledge
> **기록하지 않은 지식은 내 것이 아니다.**<br>
> 학습한 내용을 내 언어로 정리하여 기본기(CS)를 다지고 기술의 깊이(Deep Dive)를 더합니다.

* **[UMC Study Notes Archive](https://github.com/seohyun27/umc-study-note)**: 중앙 워크북 기반 핵심 개념 요약 및 멘토링 자료
* **[CS Deep Dive Reports](https://github.com/seohyun27/cs-deep-dive-archive)**: 운영체제/컴퓨터구조 심화 보고서 (OS, Cache, Memory 등)

<br/>

## 📮 Contact
Email : canna7610@gmail.com

<br/>

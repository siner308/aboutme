`업데이트: 2023-11`

# 안정현 Jeong Hyun An
- Github. **[siner308](https://github.com/siner308)**
- Blog. **[blog.siner.io](/)**
- Email. **[siner308@gmail.com](mailto:siner308@gmail.com)**

---

# Introduce
개인을 넘어서, 팀단위 조직이 행복한 개발을 하기 위한 모든 것에 관심이 많습니다.

---

# Work Experiences

## 데브시스터즈 (2022.02 ~ 현재)
_진저랩 백엔드셀 소프트웨어 엔지니어. (구. 플랫폼셀) (2023.11 ~ 현재)_

데브시스터즈의 게임이 사용하는 공통 플랫폼인 DevPlay 개발

- 인증 관련 다양한 컴포넌트에 다양한 방법으로 기여
  - [데브시스터즈 기술블로그 - 그래서 계정 연동 하면 뭐가 좋은데?](https://tech.devsisters.com/posts/devplay-account/)
  - [Google Play Games Service](https://developer.android.com/games/pgs/overview?hl=ko) 인증 수단 추가
  - 기기 식별자를 통한 데브시스터즈 게임 간 편리한 로그인 제공
  - 초대코드 기반의 유저 인증 구현 (CBT, 런칭 초기에 사용)
  - 인게임 웹뷰 개편 (go template 기반에서 nextjs로 개편)
    - 8년된 인증서버에 붙어있던 웹뷰였고, 기존 팀 내에서 상당히 넓은 회색지대로 존재했음
    - 재구현하는 과정에서 많은 회색지대를 해소하였고, 인증서버의 리팩토링 두려움을 많이 줄였음
    - 이 과정에서 게임서버, 게임클라이언트, 모바일 SDK, 웹뷰, 플랫폼서버의 호출에 대한 이해도가 높아짐
- 크로스 게임 프로모션(CGP) 서버구조 개편
  - 후에 이어질 API 기반 서버구조로 개편하기에 앞서, 발생하고 있던 성능 이슈 개선
    - 의존성을 가지는 다양한 서버에서 발생하는 N+1 문제 해결
    - 레디스 캐시를 잘못 사용하고 있어서 다양한 이슈가 생기고 있었는데, 위의 성능 개선으로 인해 캐시를 서비스에서 사용하지 않도록 할 수 있었음
  - 게임-플랫폼 서버간의 통신 없이 게임서버가 찍는 로그를 기반으로 동작하던 구조에서, 게임서버에서 직접 API를 찌르도록 구조 변경
    - 기존에 게임서버에서 찍고있던 로그를 기반으로 기능을 제공한다는 멋진 아이디어에서 시작했지만, 이후 다양한 기능을 제공하기 위해 로그 스키마를 위해 다양한 이해관계자가 프로젝트에 불필요하게 참여하게 되는 등 비효율적인 구조가 되었고, API 기반으로 전환하면서 절차가 많이 간소화됨
  - 유저가 게임간 연계되는 프로모션의 보상을 받기 위해서는 하나의 계정으로 여러 게임을 묶어주는 계정연동이 필수적인데, 이 과정에서 발생하는 다양한 이슈가 있었음. 해당 프로젝트를 주도적으로 진행하면서, 기존에 가지고있던 문제점들의 원인을 파악하고 가시화함
- 인프라 개편
  - 사내 인프라 조직에서 만들어 둔 테라폼 기반의 모듈로 생성한 쿠버네티스 클러스터에 기존 서비스 이전
    - 다양한 쿠버네티스 클러스터에 흩어져있던 서비스를 하나의 클러스터로 옮기는 과정에서, 통일되어있지 않던 차트를 통일함
    - 이때 인프라 지식이 많이 늘었고, 이후 다양한 작업을 진행하는 데 도움이 됨
  - 새로운 게임에서 타 게임과 독립된 플랫폼 환경이 필요하여, 기존 서버들을 새로 띄우는 작업을 함
    - 이 과정에서 one platform 의존적인 구조였던 문제점들을 발견하고 개선함
- 사전예약 서버 개발 및 리팩토링
  - 각 게임의 N주년, CBT, 런칭 등 다양한 이벤트를 위한 사전예약 서버 개발
  - 수개월에 한번씩 진행하던 이벤트였고 그때마다 기여하는 사람이 달랐기 때문에, 각 도메인마다 모델을 정의하는 방법이 달랐고, 재사용 가능해야 하는 email/sms 발송 관련 API가 특정 이벤트 관련 데이터를 받도록 설계되어있어서 매번 코드를 변경해야 하는 구조였음
    - 코드를 하나의 패턴으로 통일하고, email/sms 발송 코드를 특정 이벤트에 디펜던트하지 않도록 리팩토링함

  `go` `nextjs` `kubernetes` `terraform` `github-actions` `helm` `redis` `mysql` `grpc` `aws` `datadog`

_진저랩 웹서비스셀 소프트웨어 엔지니어. 테크리드 (현. 웹콘솔셀) (2022.02 ~ 2023.11)_

- 사내 BI 서비스 런칭 및 유지보수 (2022.02 ~ 2023.09)
  - [데브시스터즈 기술블로그 - 웹 개발자의 데이터 애플리케이션 flow 효율화하기](https://tech.devsisters.com/posts/dash-data-flow/)
  - 복잡한 비즈니스 로직에도 효율적인 구조를 가지기 위한 DSL 설계 및 개발
- 웹콘솔 개발 (2023.08 ~ )
  - 사내 인오피스 제품들을 통합된 경험으로 제공하기 위한 제품
  - Micro frontend 아키텍처 기반의 Poc 및 구현

  `python(dash)` `webpack5(module federation)` `nextjs` `nodejs` `mysql` `kubernetes` `terraform` `argocd` `github-actions` `helm`


## 크리에이트립 (2020.06 ~ 2022.02)
_프로덕트팀 백엔드 개발자_

개발팀 규모: 10명 내외 (Backend, Frontend, App(Cross Platform))

MAU: 180만

- Backend API
  - 기존기능 유지보수 및 고도화를 통한 레거시 청산
    - koa → nestjs API 마이그레이션 및 고도화 (OAuth 로그인, 소셜통합 등)
    - 데이터베이스 구조 개선
  - 신사업(TBA) 데이터베이스 모델링 및 비즈니스 로직 구현
- Pipeline, Batch
  - sitemap 생성기 개발
  - 검색 API를 위한 키워드 관리 파이프라인 개발
    - elasticsearch tokenizer를 활용
  - error tracing을 위한 request data 적재 파이프라인 개발
- Infra
  - on-premise → ecs 무중단 마이그레이션 및 유지보수
  - 실시간 slack 모니터링 시스템 구축으로 monitoring 고도화

`graphql` `nestjs` `mariadb` `elasticsearch` `aws ecs` `aws lambda` `github-actions` `jest`

## baselabs (2019.11 ~ 2020.06)
_웹 개발자_

백엔드 개발자 2명으로 구성된 스타트업

- 스트리머, 시청자를 위한 웹 페이지 개발 (프론트엔드)
  - OAuth 로그인
  - 미션 등록 및 각종 오버레이 설정을 위한 대시보드 개발
- IRC 데이터 수집
  - 라이브 방송 채팅 데이터 수집 및 elasticsearch 적재
  - Kibana 시각화 대시보드 작성
  - 키워드 알림을 통한 모니터링
- 미션 오버레이 웹 서비스 백엔드 및 프론트엔드 개발
  - socket 통신을 통해 새로고침 없이 re-render 가능한 스트리머 방송용 화면 제공
  - Google TTS를 활용한 알림 메시지 제공
  - API → Socket 통신 → 프론트 렌더링

`websocket` `react` `express` `mysql` `elasticsearch` `google tts`

## 아이넷캅 (2018.05 ~ 2019.11)
_백엔드 개발자_

개발팀 규모: 5명 내외 (Backend, Frontend, Android)

MAU: 50만

- 안드로이드 안티바이러스 앱 T가드 (SKT) 서버 유지보수
  - SKT 내부에 위치한 서버에서 자체적으로 운영중인 서버로 API migration
- 머신러닝 Feature 추출용 Binary 빌드, 배포 파이프라인 설계 및 개발
  - Script 작성, Slack API를 통한 파일 업로드
  - 자동으로 생성되는 Binary를 통하여 개발단계에서의 테스트 편의성이 대폭 증가함
- B2B용 악성 APK 관리 페이지 개발
  - 앱 업로드시 ML검사하여 DB최신화하고 새로운 DB를 배포하는 파이프라인 설계 및 개발
  - 오퍼레이터 페이지, 사용 가이드라인 제공
- 안드로이드 앱 악성유무 검사를 위한 MSA API 개발
  - ML엔지니어로부터 모델을 받아서 배포
- On-Premise 인프라 관리
  - Jira, Confluence, Gitlab, Jenkins, Docker Registry, Nextcloud, Slack chatbot

`django` `docker` `nginx` `postgresql` `kong` `elasticsearch`

---

# Toy Projects

## 떡볶이맵 (2021.05 ~ 2024.07)
- 대한민국 어디서든 떡볶이를 빠르게 맛보기 위한 지도 서비스
- 홈서버를 통해 운영하였으나, 현재 supabase 기반으로 마이그레이션 상태
- 초기에는 크롤링 언어와 백엔드 언어를 python으로 통일하여 운영함


- Page. [https://ttbkk.com](https://ttbkk.com)
- Github
  - [frontend](https://github.com/ttbkk-univ/ttbkk-web)
  - [backend python](https://github.com/ttbkk-univ/ttbkk-server)
  - [backend spring](https://github.com/ttbkk-univ/ttbkk-spring)


- Crawling: `python` `selenium`
- Frontend: `react(vite)` `recoil` `tanstack/query` `mui/material` `kakao map` `google oauth`
- Infrastructure: `docker` `route53` `cloudfront` `s3`
- Database: `supabase`
- CI/CD: `github-actions`

## 기술 블로그 (2019.01 ~ 현재)
- Page. [https://blog.siner.io](https://blog.siner.io)
- Github
  - [blog](https://github.com/siner308/blog)
  - [blog-posts](https://github.com/siner308/blog-posts)
  - [aboutme](https://github.com/siner308/aboutme)
  - [jekyll](https://github.com/siner308/jekyll-blog) (archived)
- 초기엔 jekyll로 작성된 템플릿을 fork받아서 작성하였으나 (2019.01 ~ 2020.12) jekyll에서 **글이 아닌 코드를 작성한다는 느낌**을 많이 받았고, 이로인해 새로운 글 작성에 부담을 느끼게 되었음
- 위의 문제점을 해결하고자 gatsby로 프레임을 작성하고 git submodule로 posts를 분리한 나만의 구조로 블로그를 만들게 됨
- 현재 blog-posts repo의 issues를 활용하여 초안을 작성하고 repo에서 바로 new files로 바로 파일을 업로드 하는 플로우로 글을 작성하게 되면서, ide를 사용하지 않고 빠른 속도로 글을 작성할 수 있게 되었습니다. 이미지나 동영상도 에디터에 drag&drop으로 쉽게 업로드가 가능해짐
- submodule에서의 자동배포 방법
  - netlify와 blog repo integration을 통해 blog repo의 commit 발생시 자동배포
  - blog-posts, aboutme의 commit 발생시 github-actions를 통해 netlify webhook 호출 → 자동배포

`gatsby` `graphql` `react` `netlify` `github-actions`

## 게임 커뮤니티 Slackbot, Kakao 챗봇 서버 개발 및 운영 (2018.07 ~ 현재)
- [github](https://github.com/ingress-resistance-korea/irk-bot/)
- 텍스트 명령어을 통한 실시간 게임 데이터 요청, 크롤링 후 메신저에 이미지 업로드
- 슬랙, 카카오톡, 텔레그램을 통해 다양한 채널로 운영하였음

`python` `redis` `selenium` `slack` `telegram` `kakaotalk`

## 머신러닝을 통한 프리미어리그 승부예측기 개발 (2019.01 ~ 2019.02)
- [https://github.com/siner308/epldatacenter](https://github.com/siner308/epldatacenter)
- Django를 통한 Crawling, Database Management
- Jupyter Nodebook을 통한 모델 트레이닝
- 해당 프로젝트 진행을 위한 사전 공부로 kaggle 문제풀이 다수 진행
- 사내 머신러닝 솔루션의 이해도가 높아지는데에 많은 도움이 됨

`django` `postgresql` `selenium` `jupyter-notebook`

---

# Certificate
- [AWS Certified Solutions Architect - Associate](https://www.credly.com/badges/a83e41ea-3adc-47e0-b954-e584cebd3660/linked_in?t=rvu0yy) (2023.06)
- [DevOps: Infrastructure as Code with 테라폼(Terraform) and AWS 초급, 입문편](https://www.inflearn.com/certificate/98745-325710-1797344) (인프런 2020.10)
- [Architecting with Google Kubernetes Engine: Foundations](https://www.coursera.org/account/accomplishments/verify/GWNGQT7VTJDC) (Google 스터디잼 활동 2019.07 ~ 2019.09)
- [Google Cloud Platform Fundamentals: Core Infrastructure](https://www.coursera.org/account/accomplishments/verify/GV8DZGRV94A5) (Google 스터디잼 활동 2019.07 ~ 2019.09)
- [Getting Started with Google Kubernetes Engine](https://www.coursera.org/account/accomplishments/verify/6VW6QH4AYLBS) (Google 스터디잼 활동 2019.07 ~ 2019.09)
- 정보처리기사 (2018.05)

---

# Presentation & Interview
- 🎥 [2023 NE(O)RDINARY CONFERENCE - 비전공자의 커리어 성장기](https://www.youtube.com/watch?v=BlI4F9NZNkQ)
- 🗒 [mergingkr - 좋아하는 일로 재미있게 먹고 사는 개발자 이야기](https://medium.com/@mergingkr/좋아하는-일로-ㅈㅐ미있게-먹고-사는-개발자-이야기-e2b0c73cf5d5)
---

# ETC
- 한국방송통신대학교 컴퓨터과학과 (2021.09 ~ 2023.08)
- DE&T (2016.10 ~ 2017.04)
  - FPD 및 반도체 설비 자동화제어
- 경기대학교 전자물리학과 (2011.03 ~ 2017.02)

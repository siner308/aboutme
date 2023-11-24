`업데이트: 2023-11`

# 안정현 Jeong Hyun An
- Github. **[siner308](https://github.com/siner308)**
- Blog. **[blog.siner.io](/)**
- Email. **[siner308@gmail,com](mailto:siner308@gmail.com)**

---

# Introduce
개인을 넘어서, 팀단위 조직이 행복한 개발을 하기 위한 모든 것에 관심이 많습니다.

---

# Work Experiences

## 데브시스터즈 (2022.02 ~ 현재)
_진저랩 백엔드셀 소프트웨어 엔지니어. (구. 플랫폼셀) (2023.11 ~ 현재)_

- To be updated

_진저랩 웹서비스셀 소프트웨어 엔지니어. 테크리드 (현. 웹콘솔셀) (2022.02 ~ 2023.11)_

- 사내 BI 서비스 런칭 및 유지보수 (2022.02 ~ 2023.09)
  - 복잡한 비즈니스 로직에도 효율적인 구조를 가지기 위한 DSL 설계 및 개발
    - [웹 개발자의 데이터 애플리케이션 flow 효율화하기](https://tech.devsisters.com/posts/dash-data-flow/)
  - 캐시 데이터 적재 파이프라인 개발
- 웹콘솔 개발 (2023.08 ~ )
  - 사내 인오피스 제품들을 통합된 경험으로 제공하기 위한 제품
  - micro frontend 아키텍처 기반의 Poc 및 구현
- ETC
  - [채용 페이지](https://careers.devsisters.com) 유지보수
  - 사내 라이브 스트리밍 서비스를 scalable 하도록 구조 개선
  - 디자인시스템 코드리뷰
  - ISMS 대응

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

## 떡볶이맵 (2021.05 ~ 현재)
- 대한민국 어디서든 떡볶이를 빠르게 맛보기 위한 지도 서비스입니다.
- 집에 있는 ubuntu 서버를 통해 운영중입니다.
- 초기에는 크롤링 언어와 백엔드 언어를 python으로 통일시켰지만, type safe, IoC 등의 이점을 누리고자 Kotlin Spring으로 마이그레이션을 진행중입니다.


- Page. [https://ttbkk.com](https://ttbkk.com)
- Github.
  - [frontend](https://github.com/ttbkk-univ/ttbkk-web)
  - [backend python](https://github.com/ttbkk-univ/ttbkk-server)
  - [backend spring](https://github.com/ttbkk-univ/ttbkk-spring)


- backend, crawling: `django` `nginx` `selenium`
- backend v2 (예정): `kotlin` `spring` `flyway` `kotest`
- frontend: `react(vite)` `recoil` `tanstack/query` `mui/material` `kakao map` `google oauth`
- infrastructure: `docker` `route53` `cloudfront` `s3`
- database: `mysql` `redis`
- CI/CD: `github-actions`

## 기술 블로그 (2019.01 ~ 현재)
- Page. [https://blog.siner.io](https://blog.siner.io)
- Github.
  - [blog](https://github.com/siner308/blog)
  - [blog-posts](https://github.com/siner308/blog-posts)
  - [aboutme](https://github.com/siner308/aboutme)
  - [jekyll](https://github.com/siner308/jekyll-blog) (archived)
- 초기엔 jekyll로 작성된 템플릿을 fork받아서 작성하였으나 (2019.01 ~ 2020.12) jekyll에서 **글이 아닌 코드를 작성한다는 느낌**을 많이 받았고, 이로인해 새로운 글 작성에 부담을 느끼게 되었습니다.
- 위의 문제점을 해결하고자 gatsby로 프레임을 작성하고 git submodule로 posts를 분리한 나만의 구조로 블로그를 만들었습니다.
- 현재 blog-posts repo의 issues를 활용하여 초안을 작성하고 repo에서 바로 new files로 바로 파일을 업로드 하는 플로우로 글을 작성하게 되면서, ide를 사용하지 않고 빠른 속도로 글을 작성할 수 있게 되었습니다. 이미지나 동영상도 에디터에 drag&drop으로 쉽게 업로드가 가능해졌습니다.
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

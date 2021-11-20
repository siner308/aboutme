# 안정현 Jeong Hyun An (Siner)
- [Github](https://github.com/siner308)
- [Blog](https://blog.siner.io)
- [Facebook](https://www.facebook.com/aan308)
- [LinkedIn](https://www.linkedin.com/in/jeonghyun-an-948778185/)
- [Email](mailto:siner308@gmail.com)

# Introduce
작성예정

# Work Experiences

## creatrip (2020.06 ~ 현재)
개발팀 규모: 10명 내외 (Backend, Frontend, App(Cross Platform))

MAU: 180만

[자세한 기술스택을 포함한 채용공고는 여기에](https://career.creatrip.team/)

- backend api
  - 기존기능 유지보수 및 고도화를 통한 레거시 청산
    - koa -> nestjs API 마이그레이션 및 고도화 (OAuth 로그인, 소셜통합 등)
    - 데이터베이스 구조 개선
  - 신사업(TBA) 데이터베이스 모델링 및 비즈니스 로직 구현
- pipeline, batch
  - sitemap 생성기 개발
  - 검색 API를 위한 키워드 관리 파이프라인 개발
    - elasticsearch tokenizer를 활용
  - error tracing을 위한 request data 적재 파이프라인 개발
- infra
  - on-premise -> ecs 무중단 마이그레이션 및 유지보수
  - 실시간 slack 모니터링 시스템 구축으로 monitoring 고도화

  `graphql` `nestjs` `mariadb` `elasticsearch` `aws ecs` `aws lambda` `github-actions` `jest`

## baselabs (2019.11 ~ 2020.06)
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

## inetcop (2018.05 ~ 2019.11)
개발팀 규모: 5명 내외 (Backend, Frontend, Android)

MAU: 50만

- 안드로이드 안티바이러스 앱 T가드 (SKT) 서버 유지보수
  - skt 내부에 위치한 서버에서 자체적으로 운영중인 서버로 API migration
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

# Toy Projects

## 떡볶이맵 (2021.05 ~ 현재)
- [https://ttbkk.com](https://ttbkk.com)
- [github(frontend)](https://github.com/ttbkk-web)
- [github(backend)](https://github.com/ttbkk-server)
- 대한민국 어디서든 떡볶이를 빠르게 맛보기 위한 지도 서비스를 개발 및 운영중.

  `django` `mysql` `docker` `nginx`
  
  `kakao map` `react` `recoil` `material-ui/icons` `cloudfront` `s3` `github-actions`

## 기술 블로그 운영 (2019.01 ~ 현재)
- [https://blog.siner.io](https://blog.siner.io)
- [github(blog)](https://github.com/siner308/blog)
- [github(blog-posts)](https://github.com/siner308/blog-posts)
- [github(aboutme)](https://github.com/siner308/aboutme)
- [github(jekyll)](https://github.com/siner308/jekyll-blog) (archived)
- 초기엔 jekyll로 작성된 템플릿을 fork받아서 작성하였음. (2019.01 ~ 2020.12)
- jekyll에서 글이 아닌 '코드'를 작성한다는 느낌을 많이 받았고, 이는 블로그에 새로운 글이 작성되지 않는 문제로 이어졌음.
- 위의 문제점을 해결하고자 gatsby로 프레임을 작성하고 git submodule로 posts를 분리한 나만의 구조로 블로그를 만들었음.
- submodule에서의 자동배포 방법
  - netlify와 blog repo integration을 통해 blog repo의 commit 발생시 자동배포
  - blog-posts, aboutme의 commit 발생시 github-actions를 통해 netlify webhook 호출 -> 자동배포
- 현재 blog-posts repo의 issues를 활용하여 초안을 작성하고 repo에서 바로 new files로 바로 파일을 업로드 하는 플로우로 글을 작성하게 되었고, markdown web editor를 활용하면서 ide를 통해 블로그 글을 작성하는 끔찍한 일을 피하게 되었음. (심지어 이미지나 동영상도 에디터에 drag&drop만 하면 업로드 된다!)

`gatsby` `graphql` `react` `netlify` `github-actions`

## 게임 커뮤니티 Slackbot, Kakao 챗봇 서버 운영 경험 (2018.07 ~ 현재)
- [github](https://github.com/ingress-resistance-korea/irk-bot/)
- 텍스트 명령어을 통한 실시간 게임 데이터 요청, 크롤링 후 메신저에 이미지 업로드
- 슬랙, 카카오톡, 텔레그램을 통해 다양한 채널로 운영하였음

  `python` `redis` `selenium` `slack` `telegram` `kakaotalk`

## 머신러닝을 통한 프리미어리그 승부예측기 개발 (2019.01 ~ 2019.02)
- [https://github.com/siner308/epldatacenter](https://github.com/siner308/epldatacenter)
- Django를 통한 Crawling, Database Management
- Jupyter Nodebook을 통한 모델 트레이닝
- 최대 적중률 70% (10경기 기준)
- 해당 프로젝트 진행을 위한 사전 공부로 kaggle 문제풀이 다수 진행
- 사내 머신러닝 솔루션의 이해도가 높아지는데에 큰 요인이 됨

  `django` `postgresql` `selenium` `jupyter-notebook` `kaggle`

# Certificate
- [DevOps: Infrastructure as Code with 테라폼(Terraform) and AWS 초급, 입문편](https://www.inflearn.com/certificate/98745-325710-1797344) (인프런 2020.10)
- [Architecting with Google Kubernetes Engine: Foundations](https://www.coursera.org/account/accomplishments/verify/GWNGQT7VTJDC) (Google 스터디잼 활동 2019.07 ~ 2019.09)
- [Google Cloud Platform Fundamentals: Core Infrastructure](https://www.coursera.org/account/accomplishments/verify/GV8DZGRV94A5) (Google 스터디잼 활동 2019.07 ~ 2019.09)
- [Getting Started with Google Kubernetes Engine](https://www.coursera.org/account/accomplishments/verify/6VW6QH4AYLBS) (Google 스터디잼 활동 2019.07 ~ 2019.09)
- 정보처리기사 (2018.05)

# ETC
- 한국방송통신대학교 재학중 (2021.09 ~ 현재)
  - 컴퓨터공학과
- DE&T (2016.10 ~ 2017.04)
  - FPD 및 반도체 설비 자동화제어
- 경기대학교 졸업 (2011.03 ~ 2017.02)
  - 전자물리학과

# 🍀 Git 설정 & 프로젝트 관리 시작하기

## 🧸 Git

<br>

### ⛄ Git 최초 설정

#### Git 전역으로 사용자 이름과 이메일 주소를 설정

- GitHub 계정과는 별개
- Git을 협업할 때 사용
  - 각 작업들마다 누가 했고, 연락수단을 위해

#### 터미널 프로그램 (GitBash, iTerm2)에서 명령어 실행

- git config --global user.name "(본인 이름)"
- git config --global user.email "(본인 이메일)"

#### 명령어로 확인

- git config --global user.name
- git config --global user.email

#### 기본 브랜치명 변경

- git config --global init.defaultBranch main

<br>

### ⛄ 프로젝트 생성 & Git 관리 시작

해당 폴더에서 명령어 입력

- git init
- 폴더 숨김모드로 .git 폴더 생성 확인
- ⭐ 이 폴더를 지우면 Git 관리내역 삭제됨 (현 파일들은 유지)

#### 상태 확인

- git status

<br>

### ⛄ 소스트리

#### 현존하는 저장소 추가

= 소스트리에 폴더를 드래그하거나, `로컬 저장소 추가`

#### Git이 관리하는 저장소 새로 만들기

- .git 폴더 삭제 후 진행
- 소스트리에 폴더를 드래그하거나, `로컬 저장소 생성`

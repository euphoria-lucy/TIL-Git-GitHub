# 🍀 Git Hooks

<br>

## 🧸 Git **Hooks**

Git 상의 이벤트마다 자동으로 실행될 스크립트를 지정함

<br>

### ⛄ Git Hooks 폴더 보기

프로젝트 폴더 내 `.git` > `hooks` 폴더 확인

- 파일 끝에 `.sample` 을 없애면 훅 실행파일이 됨

<br>

## 🧸 **gitmoji-cli** 로 활용 예 보기

<br>

### ⛄ gitmoji-cli 설치

윈도우

- **Node.js** 로 설치
- 터미널에서 설치 : `npm i - g gitmoji-cli`

맥

- `brew` 로 설치 : `brew install gitmoji`

<br>

### ⛄ 프로젝트의 훅에 적용

프로젝트 폴더에서 명령어 실행

```bash
gitmoji -i
```

- `hooks` 폴더에 추가된 파일 확인하기
- 프로젝트에 수정 뒤 `git add .` , `git commit` 하여 진행
- 커밋 추가 뒤 push 하여 GitHub에서 확인

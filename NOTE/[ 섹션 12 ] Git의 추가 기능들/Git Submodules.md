# 🍀 Git Submodules

<br>

## 🧸 서브모듈

- 프로젝트 폴더 안에 **또 다른 프로젝트**가 포함될 때 사용
- 여러 프로젝트에 사용되는 공통모듈일 때 유용

<br>

## 🧸 사용해보기

<br>

### ⛄ 두 개의 프로젝트 생성

- `main-project` , `submodule`
- 양쪽 모두 파일 생성 및 작성 뒤 커밋
- 두 프로젝트 모두 GitHub에 각각 레포지토리 만들어 올리기

<br>

### ⛄ `main-project` 에 서브모듈로 `submodule` 프로젝트 추가

`main-project` 디렉토리상 터미널에서 명령어 실행

```bash
git submodule add (submodule의 GitHub 레포지토리 주소) (하위폴더명, 없을 시 생략)
```

- 프로젝트 폴더 내 `submodule` 폴더와 `.gitmodules` 파일 확인
- 스테이지된 변경사항 확인 뒤 커밋
- 양쪽 모두 수정사항 만든 뒤 `main-project` 에서 `git status` 로 확인
  `submodule` 의 변경사항은 포함되지 않음 확인
- `main-project` 에서 변경사항 커밋 뒤 푸시
- `submodule` 에서 변경사항 커밋 뒤 푸시
- `main-project` 에서 상태 확인
- `main-project` 에서 커밋, 푸시 뒤 GitHub에서 확인

<br>

### ⛄ 서브모듈 업데이터

1. `main-project` 새로운 곳에 clone 하기
2. 명령어들로 서브모듈 init 후 클론

```bash
git submodule init (특정 서브모듈 지정시 해당 이름)
```

```bash
git submodule update
```

3. GitHub에서 `submodule` 에 수정사항 커밋
   `main-project` 에서 명령어로 업데이트

```bash
git submodule update --remote
```

- 서브모듈 안에 또 서브모듈이 있을 시 : `--recursiv` 추가

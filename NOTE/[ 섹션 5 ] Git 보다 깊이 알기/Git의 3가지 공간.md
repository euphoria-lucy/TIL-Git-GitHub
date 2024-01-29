# 🍀 Git의 3가지 공간

<br>

## 🧸 Git의 3가지 공간

<br>

### ⛄ Working directory

- untracked : Add 된 적 없는 파일, ignore 된 파일
- tracked : Add 된 적 있고 변경내역이 있는 파일
- `git add` 명령어로 Staging area로 이동

<br>

### ⛄ Staging area

- 커밋을 위한 준비 단계
  - 예) 작업을 위해 선택된 파일들
- `git commit` 명령어로 repository로 이동

<br>

### ⛄ Repository

- `.git directory` 라고도 불림
- 커밋된 상태

<br>

## 🧸 파일의 삭제와 이동

<br>

### ⛄ git **rm**

<br>

### ⛄ git **mv**

<br>

### ⛄ 파일을 `staging area` 에서 `working directory` 로

```bash
git restore --staged (파일명)
```

- `--staged` 를 빼면 `working directory` 에서도 제거
- 과거 : `git reset HEAD (파일명)

<br>

## 🧸 **reset** 의 세 가지 옵션

- --soft : `repository` 에서 `staging area` 로 이동
- --mixed (Default) : `repository` 에서 `working directory` 로 이동
- --hard : 수정사항 완전히 삭제

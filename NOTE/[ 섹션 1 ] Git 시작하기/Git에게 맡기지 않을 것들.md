# 🍀 Git에게 맡기지 않을 것들

## 🧸 Git

<br>

### ⛄ Git의 관리에서 특정 파일/폴더를 배제해야 할 경우

- 포함할 필요가 없을 때
  - 자동으로 생성 또는 다운로드되는 파일들 (빌드 결과물, 라이브러리)
- 포함하지 말아야 할 때

  - 보안상 민감한 정보를 담은 파일

- 💡 **.gitignore 파일**을 사용해서 배제할 요소들을 지정할 수 있음

<br>

### ⛄ .gitignore 사용

- `.gitignore` 파일 생성

```bash
git status
```

로 상태 확인

<br>

### ⛄ .gitignore 형식

```bash
# 이렇게 #를 사용해서 주석

# 모든 file.c
file.c

# 최상위 폴더의 file.c
/file.c

# 모든 .c 확장자 파일
*.c

# .c 확장자지만 무시하지 않을 파일
!not_ignore_this.c

# logs란 이름의 파일 또는 폴더와 그 내용들
logs

# logs란 이름의 폴더와 그 내용들
logs/

# logs 폴더 바로 안의 debug.log와 .c 파일들
logs/debug.log
logs/*.c

# logs 폴더 바로 안, 또는 그 안의 다른 폴더(들) 안의 debug.log
logs/**/debug.log
```

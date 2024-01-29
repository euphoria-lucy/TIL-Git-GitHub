# 🍀 log 더 자세히 알아보기

<br>

## 🧸 옵션들을 활용한 다양한 사용법

<br>

### ⛄ 각 커밋마다의 변경사항 함께 보기

```bash
git log -p
```

<br>

### ⛄ 최근 n개 커밋만 보기

```bash
git log -(갯수)
```

<br>

### ⛄ 통계와 함께 보기

```bash
git log --stat
```

- 더 간략히 : `--shortstat`

<br>

### ⛄ 한 줄로 보기

```bash
git log --oneline
```

- `--pretty=oneline --abbrev-commit` 의 줄임

<br>

### ⛄ 변경사항 내 단어 검색

```bash
git log --S (검색어)
```

- `George` 로 검색

<br>

### ⛄ 커밋 메시지로 검색

```bash
git log --grep (검색어)
```

<br>

### ⛄ 자주 사용되는 그래프 로그 보기

```bash
git log --all --decorate --online --graph
```

- `--all` : 모든 브랜치 보기
- `--graph` : 그래프 표현
- `--decorate` : 브랜치, 태그 등 모든 레퍼런스 표시
  - `--decorate=no`
  - `--decorate-short` : 기본
  - `--decorate=full`

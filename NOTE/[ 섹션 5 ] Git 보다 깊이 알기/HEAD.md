# 🍀 HEAD

<br>

## 🧸 Git의 **HEAD**

현재 속한 브랜치의 가장 최신 커밋

<br>

### ⛄ `checkout` 으로 앞뒤 이동해보기

```bash
git checkout HEAD^
```

- `^` 또는 `~` : 갯수만큼 이전으로 이동

<br>

- ⭐ **커밋 해시** 를 사용해서도 이동 가능

  - `git checkout (커맷해시)`

<br>

- `git checkout ~` : (이동을) 한 단계 되돌리기

<br>

## 🧸 이전으로 checkout된 상태에서 소스트리로 HEAD 상태 보기

익명의 브랜치에 위치함을 알 수 있음

- `checkout` 으로 이전으로 돌아간 뒤
  - 기존 브랜치로 돌아오기 : `git switch (브랜치명)`
  - 새 브랜치 만들어보기
  - 새 커밋 만들어보기

<br>

## 🧸 HEAD 사용하여 reset 하기

```bash
git reset HEAD (원하는 단계) (옵션)
```

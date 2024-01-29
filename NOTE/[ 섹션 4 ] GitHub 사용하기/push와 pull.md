# 🍀 push와 pull

<br>

## 🧸 원격으로 커밋 밀어올리기 (**push**)

```bash
git push
```

- 이미 `git push -u origin main` 으로 대상 원격 브랜치가 지정되었기 때문에 가능

<br>

## 🧸 원격의 커밋 당겨오기 (**pull**)

```bash
git pull
```

<br>

## 🧸 **pull** 할 것이 있을 때 **push** 를 하면?

- push 할 것이 있을 시 pull 하는 두 가지 방법
  - `git pull --no rebase` - **merge** 방식
  - `git pull --rebase` - **rebase** 방식

<br>

## 🧸 로컬의 내역 강제 push 해보기

- 로컬의 내역 충돌 전으로 `reset`
- 명령어로 원격에 강제 적용

```bash
git push --force
```

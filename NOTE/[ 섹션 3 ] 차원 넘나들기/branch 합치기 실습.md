# 🍀 branch 합치기 실습

<br>

## 🧸 **merge** 로 합치기

```bash
git merge (브랜치명)
```

- `:wq` 로 자동입력된 커밋 메시지 저장하여 마무리

<br>

### ⛄ `merge` 는 `reset` 으로 되돌리기 가능

- `merge` 도 하나의 커밋
- `merge` 하기 전 해당 브랜치의 마지막 시점으로

<br>

### ⛄ 병합된 브랜치 삭제

```bash
git branch -d (브랜치명)
```

<br>

## 🧸 **rebase** 로 합치기

`A` 브랜치를 `B` 브랜치로 **rebase**

- `A` 브랜치로 이동
  ```bash
  git rebase (B 브랜치명)
  ```
- `B` 브랜치로 이동 후 `A` 의 시점으로 **fast-forward**

  ```bash
  git merge (B 브랜치명)
  ```

- `B` 브랜치 삭제

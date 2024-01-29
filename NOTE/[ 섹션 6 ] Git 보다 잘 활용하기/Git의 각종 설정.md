# 🍀 Git의 각종 설정

<br>

## 🧸 **global** 설정과 **local** 설정

config를 **--global** 과 함께 지정하면 전역으로 설정됨

<br>

## 🧸 설정값 확인

현재 모든 설정값 보기

```bash
git config (global) --list
```

<br>

에디터에서 보기 _(기본 : vi)_

```bash
git config (global) -e
```

<br>

기본 에디터 수정

```bash
git config --global core.editor "code --wait"
```

- 또는 `code` 자리에 원하는 편집 프로그램의 .exe 파일 경로 연결
- `--wait` : 에디터에서 수정하는 동안 CLI를 정지
- 💡 `git commit` 등의 편집도 지정된 에디터에서 열게 됨

<br>

## 🧸 유용한 설정들

줄바꿈 호환 문제 해결

```bash
git config --global core.autocrlf (윈도우: true / 맥: input)
```

<br>

`pull` 기본 전략 `merge` 또는 `rebase` 로 설정

```bash
git config pull.rebase false
```

```bash
git config pull.rebase true
```

<br>

기본 브랜치명

```bash
git config --global init.defaultBranch main
```

<br>

push시 로컬과 동일한 브랜치명으로

```bash
git config --global push.default current
```

<br>

## 🧸 단축키 설정

```bash
git config --global alias.(단축키) "명령어"
```

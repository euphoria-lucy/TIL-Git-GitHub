# 🍀 SSH로 접속하기

<br>

## 🧸 **SSH** 프로토콜을 통한 인증

- **공개키** 암호화 방식 활용
- username과 토큰 사용할 필요 없음
- 컴퓨터 자체에 키 저장

<br>

## 🧸 SSH 키 등록하기

- 계정의 `Settings` - `SSH and GPG keys`
- 해당 페이지의 가이드 참조

<br>

### ⛄ SSH키 존재 여부 확인

- 터미널 (윈도우의 경우 Bash Shell) 에서 `~/.ssh` 로 이동

```bash
cd ~/.ssh
```

<br>

- `id_rsa.pub` , `id_ecdsa.pub` , `id_ed25519.pub` 파일 중 하나 존재 여부 확인

```bash
ls
```

<br>

### ⛄ SSH 키 생성

- 터미널 (윈도우의 경우 Bash Shell) 에서 키 생성

```bash
ssh-keygen -t ed25519 -C "(이메일주소)"
```

<br>

- 원할 시 `passphrase` 입력

<br>

### ⛄ GitHub에 키 등록

- 공개키 열람하여 복사

```bash
cat ~/.ssh/id_ed25519.pub
```

<br>

- `New SSH Key` 클릭하여 키 이름과 함께 등록

<br>

### ⛄ SSH로 사용해보기

- 원격을 SSH 주소로 변경한 뒤 테스트

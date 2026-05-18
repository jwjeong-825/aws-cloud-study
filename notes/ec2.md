# EC2

## What is EC2?

EC2(Elastic Compute Cloud)는 AWS에서 제공하는 가상 서버 서비스이다.

사용자는 원하는 사양의 Linux 서버를 생성하고 운영할 수 있다.

---

## Features

- 가상 서버 생성 가능
- 다양한 instance type 제공
- Ubuntu / Amazon Linux 등 OS 선택 가능
- 스토리지 및 네트워크 설정 가능

---

## AMI

AMI(Amazon Machine Image)는 서버 생성용 이미지이다.

예시:
- Ubuntu
- Amazon Linux
- RedHat

---

## Instance Type

서버 성능을 결정한다.

예시:

```txt
t3.micro
```

- CPU
- Memory
- Network 성능

등이 결정된다.

---

## Key Pair

EC2 SSH 접속용 인증 키

```txt
.pem
```

파일을 다운로드하여 사용한다.

---

## Public IP

외부 인터넷 접속용 IP 주소

브라우저 또는 SSH 접속에 사용된다.

---

## Apache Installation

```bash
sudo apt update -y
sudo apt install apache2 -y
```

웹 서버 설치 가능

---

## What I Practiced

- EC2 instance 생성
- Ubuntu 서버 생성
- key pair 생성
- public IP 접속
- Apache 설치
- Linux 서버 원격 접속 실습

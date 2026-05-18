# NAT Gateway

## What is NAT Gateway?

NAT Gateway는 private subnet의 인스턴스가 인터넷에 접근할 수 있도록 해주는 AWS 서비스이다.

외부에서는 private subnet 내부 인스턴스에 직접 접근할 수 없다.

---

## Why NAT Gateway is Needed

Private subnet은 Internet Gateway와 직접 연결되지 않는다.

따라서:
- apt install
- package download
- software update

등 인터넷 연결이 필요한 작업이 불가능하다.

NAT Gateway를 사용하면 outbound 인터넷 통신 가능하다.

---

## Features

- private subnet 인터넷 접근 지원
- 외부에서 직접 inbound 접근 불가
- 보안 강화 가능

---

## Architecture

```txt
Internet
   ↓
Internet Gateway
   ↓
Public Subnet
   ↓
NAT Gateway
   ↓
Private Subnet
```

---

## Usage Example

- WAS 서버
- Database 서버
- 내부 시스템 서버

등에 사용 가능

---

## What I Practiced

- NAT Gateway 생성
- routing table 연결
- private subnet 인터넷 연결
- WEB/WAS 구조 이해

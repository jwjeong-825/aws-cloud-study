# Security Group

## What is Security Group?

Security Group은 AWS EC2 인스턴스에 적용되는 가상 방화벽이다.

인바운드와 아웃바운드 트래픽을 제어한다.

---

## Features

- EC2 인스턴스 단위 적용
- 허용(allow) 규칙 기반
- 상태 저장(stateful) 방식

---

## Inbound Rule

외부에서 인스턴스로 들어오는 트래픽 제어

예시:
- HTTP : 80
- HTTPS : 443
- SSH : 22

---

## Outbound Rule

인스턴스에서 외부로 나가는 트래픽 제어

기본적으로 모든 outbound 허용 상태

---

## SSH Port

```txt
TCP 22
```

Linux 서버 원격 접속용 포트

보안을 위해:
- 0.0.0.0/0 전체 허용 대신
- 내 IP만 허용 권장

---

## HTTP Port

```txt
TCP 80
```

웹 서버 접근용 포트

---

## What I Practiced

- security group 생성
- inbound/outbound rule 설정
- HTTP 80 포트 설정
- SSH 22 포트 설정
- EC2 보안 설정 실습


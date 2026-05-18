# VPC

## What is VPC?

VPC(Virtual Private Cloud)는 AWS에서 제공하는 가상 네트워크 공간이다.

사용자는 자신만의 네트워크 환경을 구성하고 AWS 리소스를 배치할 수 있다.

---

## Features

- 독립적인 네트워크 환경 제공
- IP 주소 범위 설정 가능
- subnet 구성 가능
- routing table 설정 가능
- internet gateway 연결 가능

---

## CIDR

CIDR(Classless Inter-Domain Routing)은 IP 주소 범위를 표현하는 방식이다.

예시:

```txt
10.0.0.0/16
```

- 앞 부분 : 네트워크 주소
- /16 : subnet mask

사용 가능한 IP 범위를 정의한다.

---

## Public / Private Subnet

### Public Subnet

인터넷과 직접 연결 가능한 subnet

- Internet Gateway 연결
- WEB 서버 배치 가능

---

### Private Subnet

인터넷에서 직접 접근 불가능한 subnet

- 내부 시스템 구성
- WAS / Database 서버 배치

---

## Routing Table

네트워크 트래픽의 경로를 결정한다.

Public subnet은 Internet Gateway로 연결되는 route를 가진다.

---

## Internet Gateway

VPC와 인터넷을 연결하는 gateway

Public subnet이 외부 인터넷과 통신 가능하도록 한다.

---

## What I Practiced

- AWS VPC 생성
- CIDR 설정
- public/private subnet 구성
- routing table 확인
- internet gateway 연결


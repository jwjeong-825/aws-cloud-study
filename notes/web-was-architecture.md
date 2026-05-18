# WEB / WAS Architecture

## What is WEB Server?

WEB 서버는 사용자의 HTTP 요청을 처리하는 서버이다.

정적 파일(HTML, CSS, Image 등)을 제공한다.

예시:
- Apache
- Nginx

---

## What is WAS?

WAS(Web Application Server)는 동적인 웹 애플리케이션을 실행하는 서버이다.

비즈니스 로직과 애플리케이션 처리를 담당한다.

예시:
- Tomcat
- Spring Boot
- FastAPI

---

## WEB / WAS Separation

WEB 서버와 WAS 서버를 분리하면:

- 보안 향상
- 유지보수 편리
- 확장성 증가
- 역할 분리 가능

---

## Architecture

```txt
Client
   ↓
WEB Server (Apache)
   ↓
WAS Server (Tomcat)
```

---

## Reverse Proxy

WEB 서버가 사용자의 요청을 받아 WAS 서버로 전달한다.

예시:
- Apache → Tomcat
- Nginx → FastAPI

---

## Public / Private Structure

### WEB Server

- Public Subnet 배치
- 외부 인터넷 접근 가능

### WAS Server

- Private Subnet 배치
- 내부 네트워크에서만 접근 가능

---

## What I Practiced

- WEB/WAS 구조 실습
- Apache ↔ Tomcat 연결
- Reverse Proxy 설정
- Public / Private subnet 구조 이해

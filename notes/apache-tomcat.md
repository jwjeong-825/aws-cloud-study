# Apache & Tomcat

## Apache

Apache는 대표적인 WEB 서버이다.

HTTP 요청을 처리하고 정적 파일을 제공한다.

---

## Apache Installation

```bash
sudo apt update -y
sudo apt install apache2 -y
```

---

## Apache Service

### Start

```bash
sudo systemctl start apache2
```

---

### Enable

```bash
sudo systemctl enable apache2
```

---

### Restart

```bash
sudo systemctl restart apache2
```

---

## Tomcat

Tomcat은 Java 기반 WAS(Web Application Server)이다.

동적인 웹 애플리케이션 실행 가능

---

## OpenJDK Installation

```bash
sudo apt install openjdk-17-jdk
```

---

## Tomcat Installation

```bash
sudo wget https://archive.apache.org/dist/tomcat/
```

압축 파일 다운로드 후 설치 가능

---

## Startup

```bash
sudo ./startup.sh
```

Tomcat 서버 실행

---

## WEB / WAS Connection

Apache가 Reverse Proxy 역할을 수행하여
Tomcat으로 요청 전달 가능

---

## What I Practiced

- Apache 설치
- Tomcat 설치
- OpenJDK 설치
- Apache ↔ Tomcat 연동
- Reverse Proxy 구조 이해


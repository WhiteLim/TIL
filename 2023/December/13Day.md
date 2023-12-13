# DNS 서버의 종류 
## Recursive DNS 서버
## Root DNS 서버 - ICANN
## TLD DNS 서버 - 최상위 도메인 (레지스트리)
## Authoritative DNS 서버 - 도메인 판매업체 (레지스트라)


## 흐름도
```
브라우저 -> ISP DNS 서버 (Recursive DNS 서버) -> Root DNS 서버 -> TLD DNS 서버 -> Authoritative DNS 서버 -> ISP DNS 서버 -> 브라우저 -> 호스팅서버 -> 브라우저
ㄴ 브라우저에서 도메인으로 접속 시 통신사 서버로 접근하여 어디로 가야할지 질문
ㄴ 통신사 DNS 서버는 절대 존업 서버인 Root DNS 서버로 접속 최상위 도메인 DNS 를 알려줌
ㄴ 최상위 DNS는 Authoritative DNS(레지스트라) 서버를 알려줌
ㄴ Authoritative DNS 서버는 IP를 회신함
ㄴ ISP DNS는 Authoritative DNS 서버가 준 IP를 브라우저로 회신
ㄴ 브라우저는 다시 호스팅 서버(IP) 주소로 접근
ㄴ 호스팅 서버는 결과값을 브라우저에게 리턴함
```

# Domain Learn
## Concept
1. 도메인(Domain)
```
숫자로 된 IP주소 > 쉬운 문자로 변환, 인터넷 주소 ex) naver.com
```
2. 호스팅(Hosting)
```
홈페이지를 만들기 위해 기반이 되는 공간(서버)
```
3. 네임서버(Name Server)
```
호스팅과 도메인을 연결해주는 고리, 도메인과 IP의 상호변환을 가능하게 해주는 서버
```
## Info
1. DB(Data Base)
```
데이터베이스
회사가 보유하고 있는정보 - 회원등록, 결제 등 관련 정보
```
2. Whois
```
도메인 이용자 정보(공개 정보 - 만료일, 네임서버, 상태, 등록자)
```

## Type
1. 국내도메인
```
TLD가 .kr/한국으로 끝나는 도메인
co.kr / or.kr / pe.kr / re.kr 등
```
2. 국제도메인
```
.kr/ .한국으로 끝나는 도메인을 제외한 모든 도메인
gTLD - .com/ .net/ .org/ .info 등
ccTLD - jp/ eu/ us/ cn
```

## Registrar
1. 국제 도메인 관리 기구 - ICANN
2. 레지스트리 - Registry [최상위도메인등록기관]
```
verisign - com/net
pir - org
afilias - info
등..

최상위도메인등록기관은 도메인등록자에게 판매가 불가능하며,
도매 형식으로 레지스트라와 리셀러에게 판매만 가능
```
3. 레지스트라 - Registrar [도메인등록대행기관]
```
닷네임코리아, 가비아, 호스팅케이알, 후이즈 등..
```
4. 리셀러 - Reseller [도메인등록대행제휴업체]
```
닷홈, 미리내 등..
```
5. 레지스트란트 - Registrant [도메인등록자]

## 국내도메인과 국제도메인의 차이점.
```
만료 시점 이후 유예기간 30일이 주어지는것은 동일
국제도메인은 삭제대기(복구)기간 30일이 추가로 주어지며, 복구시 159,500원 발생
복구를 안했을 시 7~15일 후 낙장
```

## DNS 설정
* A레코드(IP 주소) - 도메인 이름을 IP주소로 연결
* CNAME레코드 - 도메인 이름을 CNAME(/가 없는 영문주소)주소로 연결
* MX레코드 - 메일을 설정하는 값
* TXT레코드 - 메일 주고받는 것을 원활하게 하는 값


## Keyword
1. TLD(Top-Level Domain)
```
최상위 도메인, 도메인의 오른쪽 가장 마지막 점 다음에 위치
```
2. gTLD(generic Top-Level Domain)
```
ccTLD를 제외한 모든 도메인
```
3. ccTLD(Country code Top-Level Domain)
```
국가 도메인 - jp, us 등
```
4. DNS (Domain Name System)
```
도메인 이름들의 위치를 알아내기 위해 IP주소로 바꾸어주는 시스템
```
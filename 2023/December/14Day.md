## CDN이란?
```
Content Delivery Network의 약자로
지리적 제약 없이 전 세계 사용자에게 빨고 안전하게 콘텐츠를 전송할 수 있는 콘텐츠 전송 기술

CDN은 서버와 사용자 상의 물리적 거리를 줄여 콘텐츠 로딩에 소용되는 시간을 최소화 한다.
CDN은 각 지역에 캐시 서버(PoP, Points of Presence)를 분산 배치해 근접한 사용자에게 요청에 원본 서버가 아닌 캐시 서버가 콘텐츠를 전달
```
## GIT 명령어 모음
```
git status 현재 변경된 파일 목록 확인
git diff 파일명 현재 변경된 상세 내역 확인
git checkout 파일명 변경된 파일을 다시 되돌림
git add 파일명 특정 파일 커밋 목록 추가
git add . 변경 된 전체 파일 커밋 목록 추가
git reset HEAD 파일명 준비 영역에서 삭제
git commit -m “메세지“ 준비 영역에 추가 된 파일 커밋 진행
git reset —soft HEAD^ 커밋 취소
git merge 가지이름 해당 가지의 내용을 작업중인 가지로 합치기
git pull origin 가지이름 해당 가자의 최신 데이터 다운로드
git push origin 가지이름 해당 가지의 지금까지 커밋한 내용 업로드

— Master의 최신 코드 받아오기 명령어
git pull origin master
```
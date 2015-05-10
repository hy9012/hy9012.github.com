---
title:  "우분투에서 서브라임텍스트에 나눔 글꼴 설치"
date:   2015-05-10 22:21:00
categories: mongodb
---

#1. 다운로드 

> http://www.mongodb.org/downloads

#2. 복사하기
다운받은 폴더의 이름을 바꾼 뒤, 원하는 경로에 복사

#3. 데이터베이스 폴더 설정

데이터베이스가 들어갈 폴더를 설정
> mkdir C:\mongodb\data

#4. mongodb 단순 실행
> C:\mongodb\bin\mongod.exe --dbpath C:\mngodb\data

#5. 설정 파일

서비스 등록시 사용할 설정 파일
설정파일에 들어가는 파일들은 미리 만들어 놓아야 함
*mongod.cfg

> \# 데이터베이스 폴더
>
> dbpath = C:\mongodb\data
>
> \# mongdb 포트
>
>port = 27017
>
> \# 로그 파일
>
> logpath = C:\mongodb\logs\mongo.log
>
> \# 웹 관리 사용
>
> rest = true

#6. 서비스 등록하기

* cmd.exe를 관리자 모드로 실행
> C:\mongodb\bin\mongod.exe -f C:\mongodb\mongod.cfg -install

* 웹 관리 툴 확인
> http://127.0.0.1:28017/

#7. 서비스 제거하기

> C:\mongodb\bin\mongod.exe -f C:\mongodb\mongod.cfg -remove

# 참고
> http://gyuha.tistory.com/470#recentTrackback

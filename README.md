# 주요 Git CLI 명령어
---
## 🔧 초기 설정 관련
- git config --global user.name "이름" : 사용자 이름 설정
- git config --global user.email "이메일" : 사용자 이메일 설정
- git config --list : 설정 확인

## 🗂️ 저장소 관리
- git init : 현재 디렉토리를 Git 저장소로 초기화

## 📝 변경 사항 추적
- git status : 현재 작업 상태 확인 (변경 파일 등)
- git add <파일> : 변경 파일을 스테이지 영역에 추가
- git add . : 모든 변경 파일을 스테이지에 추가
- git commit -m "커밋 메시지" : 스테이지에 있는 변경사항 커밋
※ git commit : 커밋 메시지 입력창이 자동으로 뜸. 입력 후 저장하고 닫으면 됨

## 🔄 버전 이동 & 기록 보기
- git log : 커밋 로그 보기
- git log --oneline : 한 줄 요약 로그 보기
- git checkout <브랜치명> : 다른 브랜치로 전환

## 🌿 브랜치
- git branch : 현재 브랜치 목록 확인
- git branch <이름> : 새 브랜치 생성
- git checkout -b <이름> : 브랜치 생성 + 이동
- git switch -c <브랜치치이름> : 최신 문법.
- git merge <브랜치> : 현재 브랜치에 다른 브랜치 병합
- git branch -D <이름> : 브랜치 삭제
- git push -u origin <브랜치 이름> : 브랜치 원격 저장소에 업로드.
- git push origin --delete <브랜치 이름> : 원격 저장소에 있는 브랜치 삭제. 
## ☁️ 원격 저장소
※ 원격 저장소에 업로드하기 전 반드시 github에 접속하여 새 repository 생성해야 함

- git remote add origin <repository 주소> : 현재 프로젝트를 원격 저장소와 연결
- git remote -v : 원격 저장소 목록 확인
- git push origin <브랜치> : 원격 저장소의 특정 브랜치에 업로드

## ☁️ 클론
- git clone <HTTPS주소> <만들고 싶은 폴더 명(생략가능)> : 클론하기.
- git pull : 동기화 시키기. 
- npx degit <HTTPS주소> <만들고 싶은 폴더 명(생략가능)> : 누군가의 파일을 클론하고 싶은데, .git을 빼고 클론하고 싶을때. 

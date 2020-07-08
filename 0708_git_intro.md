# git intro

## local git

1. git 다운로드 밑 설치

2. 초기화 `$ git init'

   1.  실제로는 폴더에 .git/폴더가 생성됨
   2.  버전 관리가 시작됨
   3. repo(repository)라고 부름

3. 서명 설정 

   1. `$ git config --global user.name "name"`
   2. `git config --global user.email "email@gmail.com"`

   3. 리보의 상태보기 `$ git status`

   4. stage에 올린다`$ git add` (초록색은 사진 찍을 준비가 끝난 것/ stage에 올라온 상태)

      1. 특정 파일만 올리기 `$ git add <filename>`
      2. 그냥 다 올리기 `$ git add .`

   5. snapshot (스테이지를 사진) 찍기 `$ git commit`

   6. 로그(사진첩)보기 `$ git log`

      

   ### 집 컴퓨터 세팅

   1. git 다운로드 및 설치
   2. windows 키 누루고 git bash 실행(집의 홈 폴더로 시작)
   3. `$ git config --global ...`해야 함
   4. `$ git clone <URL>`
   5.  add commit 저장 우클릭 bash here
   6. `$git commit -m '집setting 추가'`
   7. `$ git push`

   ## github

   1. 원격저장소(remote repository)

   2. local repo => remote repo 연결하기`$ git remote add origin <URL>`

   3. local 커밋을 remote 로 보내기 `$ git push origin master`

   4. `$ git push == $ git push origin master`로 단축 명령하기

       `$ git push -u origin master`해주면 된다

   5. 이후 remote repo 변경사항을 local repo 에서 반영하기 `$ git pull`

      

## TIL 관리 시나리오

1. 멀캠에 온다.
2. `$ git pull`
3. 열 공
4. 중간 중간`$git add .`& `$ git commit`
5. 집 가기 전에 `$ git push`
6. 집 도착
7. `$ git pull`
8. 복습 및 자습 (`$ git commit`)
9. 마지막으로 `$ git push`
10. 1번으로~!
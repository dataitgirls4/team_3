# team_3

> 데모데이 3조 :fire:
>
> :black_heart: 김연주 :blue_heart: 김한나 :heart: 김현진 :green_heart: 박지현 :purple_heart: 최미리

## github 사용법

### 1. dataitgirls4/team_3 원격저장소(깃헙)의 레퍼지토리를 자신의 컴퓨터 로컬에 복제(처음 1회만)

`git clone https://github.com/dataitgirls4/team_3.git`



### 2. 다른 멤버가 push한 것(이 있다고 생각하고)  pull 먼저 하고 진행할 것

#### main에서

`git checkout main`

#### 수정사항을 pull한다.

`git pull origin main`



### 3. 각자의 branch로 가서 작업하기 (나중에 main에서 합칠것)

#### 기존에 작업하던 branch가 있다면 가서 작업(ex.miree) 

`git checkout miree`

#### 		다른 branch에 있는 내용과 합치고 시작해야 된다면 병합 먼저

​	`git merge 다른branch이름`

#### 새로운 branch에서 작업하고 싶다면 branch 생성

`git branch 새로운branch이름`

#### 		기존에 있는 branch 목록을 보고싶을 땐

​	`git branch`



### 4. 작업 한 것은 원격저장소로 push

`git add .` > `git commit -m"커밋명"` > `git push`



# 데이터 설명

(2020.11.26 연주 작성)

## 1. 댓글합

- 전체 책 중 '댓글이 존재하는 책'의 정보만 있습니다.
- columns `nickname`,`rating`,`title`,`voice`,`author`,`review`,`created`,`publish`,`genre`

## 2. 전체합

- 댓글 유무와 관계 없이 팟빵오디오북에 존재하는 '모든 책'의 정보가 있습니다.
- columns `title`, `voice`, `author`, `publish`, `genre`
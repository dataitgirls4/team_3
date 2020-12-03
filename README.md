# team_3

> 데모데이 3조 :fire:
>
> :black_heart: 김연주 :blue_heart: 김한나 :heart: 김현진 :green_heart: 박지현 :purple_heart: 최미리



# 데이터 설명

(2020.12.3 연주 업데이트)

## 1. Podppang_review(11/26)

- 전체 책 중 '댓글이 존재하는 책'의 정보만 있습니다.
- columns `nickname`,`rating`,`title`,`voice`,`author`,`review`,`created`,`publish`,`genre`

## 2. Podppang_book(11/25)

- 댓글 유무와 관계 없이 팟빵오디오북에 존재하는 '모든 책'의 정보가 있습니다.
- columns `title`, `voice`, `author`, `publish`, `genre`

## 3. Naver_review(11/28)

- 팟빵오디오북에서 댓글 개수가 가장 많은 30권의 책 중, 네이버오디오북과 겹치는 13권에 대한 댓글 크롤링을 진행
- columns  `nickname`, `created`, `review`, `title`, `author`, `voice`

## 4. Welaa_review(12/1)

- 윌라 이달의 오디오북 134권에 대한 댓글 크롤링. 책 한권당 댓글 한두개정도 누락되어있을 가능성이 있음.
- columns `nickname`, `created`, `review`

## 5. Naver_event(12/2)

- 네이버 오디오클립이 진행했던 오디오북 이벤트 리스트
- columns `event_name`, `event_start`, `event_end`

# github 사용법 ​​[우리의 약속]

updated at 2020.11.29

:star: **main에서 작업X, 각자의 branch에서 작업하고. 각자가 맡은 부분은 각각의 branch로 가서 확인, 마무리된 것(공유 필요한 것)만 main에 올리기, 마무리하기 전에 공동 작업이 필요하면 그 파일만 따로 main에올려주기** :star:



## 0. 처음 1회 로컬에 원격저장소 복제

### dataitgirls4/team_3 원격저장소(깃헙)의 레퍼지토리를 자신의 컴퓨터에서 작업하려면 로컬(자신의 컴퓨터)에 원격저장소를 복제(clone)해와야 한다(처음에 1회만). 

`git clone https://github.com/dataitgirls4/team_3.git`

## 1. 원격저장소(github)에서 수정사항이 있으면 로컬(main)에 먼저 불러오기

`git pull`

(git pull을 처음하는 경우 메세지가 다르게 뜰 수 있는데 git pull origin main을 하거나 git에서 시키는대로 하다가 안되면 바로 공유해서 같이 해결하기)

### 1-1. 불러온 자료를 수정할 경우, 로컬(main)에서 원격저장소(github)으로 보내줘야함

`git add .` -> `git commit -m "커밋명(영어로)"` -> `git push`

(이거도 처음 push할 때 git push --set -upstream 블라블라 등 다른거 뜰 수 있는데 git이 시키는대로 입력해보고도 안되면 공유)

## 2. 불러온 자료를 확인만하고 각자의 branch에서 작업하기

로컬에서 자신(miree)의 branch로 이동: `git checkout miree` -> 이렇게 하면 git에 (main)이었던 것이 (miree)로 바껴야한다.

로컬(miree)에서 수정한 사항을 원격저장소(branch:miree)에 저장해주고 다른 사람들도 볼 수 있게 하려면: `git add .` -> `git commit -m "커밋명(영어로)"` -> `git push`

## 3. 내가 작업 완료한(또는 함께 수정하고 싶은) 파일만 따로 main에 올리고 싶을 땐

좀 불편하지만 아는 방법으로 확실하게 갑시다..

1. 로컬(miree)에서 해당 파일을 복사하고

2. 로컬(main)으로 이동: `git checkout main`
3. 로컬(main)에 해당 파일 붙여 넣기
4. 로컬에서 수정사항 생겼으니 원격저장소(main)에 push해서 저장해주기: `git add .` -> `git commit -m"커밋명(영어로)"` -> `git push`

---

-----

## :construction: github 작업할 때 유의 사항

### - 다른 멤버가 push한 것이 있으면(commit 내역으로 확인 가능) pull 먼저 하고 진행할 것

#### main에서

`git checkout main`

#### 수정사항을 pull한다.

`git pull origin main` (최초)

(이후) `git pull`

###  - 각자의 branch로 가서 작업하기 (나중에 main에서 합칠것)

#### 기존에 작업하던 branch가 있다면 가서 작업(ex.브랜치이름: miree) 

`git checkout miree`

#### 		다른 branch에 있는 내용과 합치고 시작해야 된다면 병합 먼저

​	`git merge 다른branch이름`

#### 새로운 branch에서 작업하고 싶다면 branch 생성

`git branch 새로운branch이름`

#### 		기존에 있는 branch 목록을 보고싶을 땐

​	`git branch`

### - 작업 한 것은 원격저장소로 push

`git add .` > `git commit -m"커밋명"` > `git push`



---

# 

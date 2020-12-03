# 데이터 설명

(2020.12.1 연주 업데이트)

## 1. 댓글합(11/26)

- 전체 책 중 '댓글이 존재하는 책'의 정보만 있습니다.
- columns `nickname`,`rating`,`title`,`voice`,`author`,`review`,`created`,`publish`,`genre`

## 2. 전체합(11/25)

- 댓글 유무와 관계 없이 팟빵오디오북에 존재하는 '모든 책'의 정보가 있습니다.
- columns `title`, `voice`, `author`, `publish`, `genre`

## 3. naver_review(11/28)

- 팟빵오디오북에서 댓글 개수가 가장 많은 30권의 책 중, 네이버오디오북과 겹치는 13권에 대한 댓글 크롤링을 진행
- columns  `nickname`, `created`, `review`, `title`, `author`, `voice`

## 4. naver_imsi_review(11/30)

- 네이버 인기책 100권에 대한 댓글 크롤링. 단, 전체 댓글이 아니라 첫번째 페이지에서 노출되는 리뷰들만 가져왔다.
- columns `'nickname'`,` 'created'`, `'review'`, `'title'`, `'author'`, `'voice'`

## 5. millie_review(12/1)

- 밀리의 서재 인기책 30권에 대한 댓글 크롤링
- columns `nickname`, `created`, `review`

## 6. welaa_review(12/1)

- 윌라 이달의 오디오북 134권에 대한 댓글 크롤링. 책 한권당 댓글 한두개정도 누락되어있을 가능성이 있음.
- columns `nickname`, `created`, `review`
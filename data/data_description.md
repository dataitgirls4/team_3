# 데이터 설명

(2020.12.06 Update)

## 1. Podppang_review(11/26)

- 전체 책 중 '댓글이 존재하는 책'의 정보만 있습니다.
- columns `nickname`,`rating`,`title`,`voice`,`author`,`review`,`created`,`publish`,`genre`

## 2. Podppang_book(11/25)

- 댓글 유무와 관계 없이 팟빵오디오북에 존재하는 '모든 책'의 정보가 있습니다.
- columns `title`, `voice`, `author`, `publish`, `genre`

## 3. Naver_review(11/30)

- 네이버 인기책 100권에 대한 댓글 크롤링. 단, 전체 댓글이 아니라 첫번째 페이지에서 노출되는 리뷰들만 가져왔다.
- columns `'nickname'`,` 'created'`, `'review'`, `'title'`, `'author'`, `'voice'`

## 4. Welaa_review(12/1)

- 윌라 이달의 오디오북 134권에 대한 댓글 크롤링. 책 한권당 댓글 한두개정도 누락되어있을 가능성이 있음.
- columns `nickname`, `created`, `review`

## 5. Naver_event(12/2)

-  네이버 오디오클립에서 진행했던 오디오북 이벤트에 대한 정보 크롤링.

-  columns `event_name`, `event_start`, `event_end`

## 6. Podbbang_event(12/1)
-  팟빵 오디오북에서 진행했던 이벤트에 대한 정보 크롤링.
=  columns 'event_name', 'event_period

## 7. Podbbang_audio_review_event(12/1)
-  팟빵 오디오북에서 진행했던 이벤트 중 오디오북 댓글 이벤트에 대한 정보 크롤링.
=  columns 'event_name', 'event_period, 'event_book'

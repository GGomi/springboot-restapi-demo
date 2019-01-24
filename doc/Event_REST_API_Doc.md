# "Event" REST API DOC
이벤트 조회, 등록, 수정 API

## GET /api/events/
이벤트 목록조회 REST API(로그인 안한 상태)
- 응답에 보여줘야할 데이터
    - 이벤트목록
    - 링크
        - self
        - profile (이벤트 목록 조회 API문서로 링크)
        - get-an-event (이벤트 하나 조회하는 API 링크)
        - next (option)
        - prev (option)
        
이벤트 목록조회 REST API(로그인 안한 상태)
- 응답에 보여줘야할 데이터
    - 이벤트목록
    - 링크
        - self
        - profile (이벤트 목록 조회 API 문서로 링크)
        - get-an-event (이벤트 하나 조회하는 API 링크)
        - create-new-event (이벤트를 생성할 수 있는 API)
        - next (option)
        - prev (option)
    - 로그인한 상태??(stateless인데?)
        - 사실 Bearer헤더에 유효한 AccessToken이 들어있는 경우

## POST /api/events
- 이벤트 생성

## GET /api/events/{id}
- 이벤트 한개 조회

## PUT /api/events/{id}
- 이벤트 수정

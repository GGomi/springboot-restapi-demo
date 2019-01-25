## Event Test 작성

## @WebMvcTest
- MockMvc 빈을 자동설정해준다.
- 웹 관련 빈만 등록해준다.(슬라이싱 테스트)

## MockMvc
- Spring MVC 테스트 핵심 클래스
- 웹서버를 띄우지 않고도 Spring MVC(DispatherServlet)가 요청을 처리하는 과정을 확인할 수 있기때문에 컨트롤러 테스트용으로 자주사용된다.

## 테스트 내용
- 입력값들을 전달하면 JSON응답으로 201이 나오는지 확인
    - Location 헤더에 생성된 이벤트를 조회할 수 있는 URI가 담겨있는지 확인
    - id는 DB에 들어갈 때 자동생성된 값으로 나오는지 확인
- 입력값으로 누가 id나 eventStatus, offline, free 이런 데이터까지 주었을 때?
- Bad_Request로 응답 vs 받기로 한 값 이외는 무시
- 입력데이터가 이상한 경우 Bad_Request로 응답
    - 입력값이 이상한 경우 에러
    - 비즈니스 로직으로 검사할 수 있는 에러
    - 에러응답메시지에 에러에 대한 정보가 있어야한다.
- 비즈니스 로직 적용됐는지 응답메시지확인
    - offline과 free 값 확인
- 응답에 HATEOAS와 porfile관련 링크가 있는지 확인.
    - self(view)
    - update(만든사람은 수정가능)
    - events(목록으로 가는 링크)
- API문서 만들기
    - 요청 문서화
    - 응답 문서화
    - 링크 문서화
    - profile링크 추가




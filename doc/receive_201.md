# Event 201응답 받기

## Test 목록
- 입력값들을 전달하면 JSON응답으로 201이 나오는지 확인
    - Location 헤더에 생성된 이벤트를 조회할 수 있는 URI 담겨있는지 확인
    - id는 DB에 들어갈 때 자동생성된 값으로 나오는지 확인.

## @RestController
- @ResponseBody를 모든 메소드에 적용한 것과 동일하다.

## ResponseEntity를 사용하는 이유
- 응답코드, 헤더, 본문 모두 다루기 편한 API

## Location URI 만들기
- HATEOAS가 제공하는 linkTo(), methodOn() 사용

## mockMvc.andDo(print())
- 콘솔에서 어떤 요청과 응답을 받았는지 확인할 수 있다.
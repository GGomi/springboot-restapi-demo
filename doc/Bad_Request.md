# Bad Request (input이 아무것도 없을 때)

## @Vaild
- 컨트롤러에서 입력을 받아올 때 검증을 수행할 수 있다.

# Bad Request (input이 잘못되었을 때)
- EventValidator라는 클래스를 통해서 컨트롤러에서 validate를 하게된다.
- @interface 를 통해서 어노테이션을 만들 수 있다.
- validate에 에러가 생기면 Errors 클래스를 통해서 에러를 담고, bad request 시킨다.
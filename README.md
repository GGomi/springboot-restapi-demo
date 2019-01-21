# REST API Demo

## 개요
REST API라는 개념이 확실하게 잡혀있지않았고, 이건 REST API가 맞다, 아니다 이런 얘기들이 많아서 학습을 시작하였습니다.


## 핵심
- **Self-Describtive** Message와 **HATEOAS**를 만족하는 제대로된 REST API를 작성하고, 이해하자. 

## 기술
- Spring Boot
- Spring-data-JPA
- Spring HATEOAS
- Spring REST Docs
- Spring Security OAuth2

## 정리내용
@Data를 Entity에 쓰지말것 
- 모든 프로퍼티를 사용해서 구현하기 때문에 상호무한참조 stackoverFlow가 발생할 위험 때문에

@WebMvcTest
- MockMvc 빈을 자동설정해줌, 웹관련 빈만 등록해준다.
- 슬라이싱 테스트, 컨트롤러 테스트로 자주 사용된다.
- 웹서버를 띄우지않아서 빠르긴하지만 단위테스트보다 빠르진않다.
- Web용 Bean만 생성해준다.

Enum을 JPA 맵핑시 주의할 것
- @Enumerated(EnumType.STRING) 권장 => ORDINARY로 설정했을때 Enum의 순서가 바뀌게되면 데이터베이스테이블 내용이 엉망진창이 된다.

## 참고
- [백기선님의 스프링기반 REST API](https://www.inflearn.com/course/spring_rest-api/)
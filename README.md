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
- Lombok
- PostgreSQL

## 정리내용
- [REST API란 무엇인가](./doc/rest_basic.md)
- [Event REST API 문서](./doc/Event_REST_API_Doc.md)
- [Create Domain](./doc/Create_Domain.md)
- [Create Business](./doc/Event_business.md)



Enum을 JPA 맵핑시 주의할 것
- @Enumerated(EnumType.STRING) 권장 => ORDINARY로 설정했을때 Enum의 순서가 바뀌게되면 데이터베이스테이블 내용이 엉망진창이 된다.



## 참고
- [백기선님의 스프링기반 REST API](https://www.inflearn.com/course/spring_rest-api/)
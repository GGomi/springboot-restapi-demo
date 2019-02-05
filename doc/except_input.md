## 입력 값 제한하기
- id 또는 입력받은 데이터로 계산해야 하는 값들은 입력을 받지 않아야한다.

## DTO -> 도메인 객체로 값 복사
- ModelMapper

## DTO를 만든 이유
- DTO를 만들지않고 어노테이션으로 해결할 수 있지만 그렇게 되면
너무 어노테이션이 많아지기때문에 따로 입력값을 받는 DTO를 따로 빼주게되었다.
- 단점은 Entity와 중복코드가 생긴다.

## DTO -> 도메인 객체로 값 복사
- Controller에서 EventDto객체를 파라미터로 받고, Event 객체로 변환해야할 때 ```ModelMapper``` 를 사용


## @SpringBootTest(통합테스트로 전환)
- mocking할 것들이 많아지면 WebMvcTest로는 테스트작성하기 힘들어지기 때문에 SpringBootTest를 사용한다.

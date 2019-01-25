# EventRepository 구현

- 스프링 데이터 JPA
    - JpaRepository 상속

- Enum을 JPA 맵핑시 주의할 것
    - @Enumerated(EnumType.STRING)
    - EnumType을 기본으로 할 시 Enum의 Index가 변하게되면 테이블이 엉망이 되어버린다.
    - 그래서 STRING 권장

- @MockBean
    - Mockito를 사용해서 mock 객체를 만들고 빈으로 등록해준다.
    - 기존 빈을 테스트용 빈이 대체한다는 점을 잊지말자.

- @Autowired
    - 생성자의 파라미터가 이미 빈에 등록되어있을때 생성자는 Autowired를 하지않아도된다.(Spring 4.3부터 가능)


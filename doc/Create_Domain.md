## 목록
- Event Domain 작성
- Event Test 작성

## @EqualsAndHashCode
- *of = {?}* 옵션을 주지않으면 Entity 간의 관계가 있을때 상호무한참조하는 일이 일어날 수 있다. 

## @Builder
- lombok annotation
- 내가 입력하는 값이 무엇인지 한눈에 알 수 있다.

## @Data를 Entity에 쓰지말것 
- 모든 프로퍼티를 사용해서 구현하기 때문에 상호무한참조 stackoverFlow가 발생할 위험 때문에
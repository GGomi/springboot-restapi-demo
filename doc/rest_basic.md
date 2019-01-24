# REST API란 무엇인가?

## API? 
- **A**pplication **P**rogramming **I**nterface

## REST?
- **RE**presentational **S**tate **T**ransfer
- 웹을 깨뜨리지않으면서 HTTP를 진화시키는 방법에 관한 논문에서 시작

## 현재 존재하는 REST API들은 진정한 REST API가 아니다!?

왜냐하면?
- **Uniform Interface** 제약조건 중에서 **Self Descriptive Message**와 **HATEOAS**가 지켜지지않기 때문이다.


## **Self Descriptive Message**
- 나는 누구인가 자기자신을 설명할 수 있어야한다.
- 확장가능한 커뮤니케이션을 가능하게한다.
- 서버와 클라이언트의 변화와 상관없이 Self Descriptive한 Message는 언제나 해석가능하다.
- 방법 - 1
    - 미디어타입을 정한다.
    - IANA에 미디어타입문서를 등록한다.
- 방법 - 2
    - profile 링크를 걸어서 사용자가 문서를 볼 수 있게한다. 

## **HATEOAS**
- 링크를 통한 상태전이가 이루어져야한다.
- late Binding, 링크는 동적으로 변경될 수 있다.

- 방법 - 1
    - data에 다양한 방법으로 하이퍼링크를 표현한다.
    - 기존API들을 많이 고쳐야한다.

- 방법 - 2
    - 헤더로 링크를 표현한다.
 
## 서버와 클라이언트는 독립적인 진화를 한다.
- REST를 만들게 된 계기이다.
- 그렇기 때문에 REST API는 Uniform Interface를 만족해야한다.

## 긴 시간에 걸쳐 진화하는 웹 애플리케이션을 위한 것이다.

 
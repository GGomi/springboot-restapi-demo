## Event 생성 API
- 입력 값
    - name
    - description
    - beginEnrollmentDateTime
    - closeEnrollmentDateTime
    - beginEventDateTime
    - endEventDateTime
    - location(optional) # 이게없으면 온라인 모임
    - basePrice(optional)
    - maxPrice(optional)
    - limitOfEnrollment

- 결과값
    - id
    - name
    - ...
    - eventStatus: 
        - DRAFT
        - PUBLISHED
        - ENROLLMENT_STARTED...
    - offline
    - free
    - _links(HATEOAS 정보)
        - profile(self descriptive Message)
        - self
        - publish
        
## basePrice와 maxPrice의 경우의 수 

basePrice|maxPrice|결과
-|-|-
0|100|선착순 등록
0|0|무료
100|0|무제한 경매
100|200|제한가 선착순 등록 
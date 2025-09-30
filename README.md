# family-community

### 컨벤션 규칙

----

- Git 커밋 메시지는 `faet`, `docs`, `test`, `refactor`, `fix`, `chore` 를 이용한다.
    - feat: 기능 추가, 개발
    - docs: 문서 작성
    - test: 테스트 코드 작성
    - refactor: 리팩토링 작업
    - fix : 버그 수정
    - chore : 그외

- 기본적으로 Java 컨벤션을 준수한다. (https://thalals.tistory.com/325)
- 클린코드 원칙에 맞춰 개발한다.
- else 를 사용하지 않는다.
- depth 는 2를 넘어가지 않는다. ex) for 메서드 내부에 if 가 있으면 depth 가 2 이다.
- 상수는 따로 분리한다.
- DTO 매핑은 Service 계층에서 진행한다.


### 디렉토리 구조


-----

- auth : 인증/인가 관련 로직을 구현한다.
- config : 애플리케이션 전역 설정 Bean 을 등록한다.
- constants : 상수를 관리한다.
- domain : 도메인 관련 로직을 구현한다.
    - controller : Rest API 계층
    - dto : dto 네이밍은 요청(xxxRequest), 응답(xxxResponse) 로 정의한다.
    - entity : 테이블과 매핑되는 클래스를 정의한다.
    - repository : 저장소역할을 담당한다.
    - service : 비지니스 로직을 담당한다.
- exception : 예외 관련 처리를 담당한다.
- infra : redis, s3, fcm 등 외부 라이브러리와 연동한다.



### 기능 명세서

----

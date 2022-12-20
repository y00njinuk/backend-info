# backend-roadmap (2022)
Step by step guide to becoming a modern backend developer in 2022

![image](https://user-images.githubusercontent.com/71953982/208684589-2a67e6ee-760b-43ff-a6ea-946ef984a765.png)

## CQRS and Event sourcing
- 이벤트 소싱은 도메인 주도 설계(DD) 커뮤니티에서 개발한 기법.
- CDC와 유사하게 애플리케이션의 상태 변화를 모두 변경 이벤트 로그로 저장한다.
- CDC와는 다음과 같은 차이가 있다.

|구분|CDC|Event sourcing|
|------|---|---|
|데이터 형식|데이터베이스 로그|이벤트 소싱|
|발행자|데이터베이스|애플리케이션|

- 또한, 이벤트 로그를 사용하면 기존 데이터를 새로운 방식으로 표현하기 위해 신규 기능용으로 분리한 읽기에 최적화 된 뷰를 구성할 수 있다.
- 이러한 개념을 CQRS(Command Query Responsiblity Segregation, 명령과 질의 책임의 분리)라고 한다.

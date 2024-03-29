# 동기식 IO란?
* 운영 체제에서의 동기 입출력(Synchronous I/O)은 입출력 작업이 완료될 때까지 프로세스의 실행을 중단시키는 방식이다.
* 이는 프로그램이 데이터를 읽거나 쓸 때 해당 작업이 끝날 때까지 기다려야 한다는 것을 의미한다.
* 즉, 데이터 전송이 완료되고 제어가 프로그램으로 돌아올 때까지 프로세스는 다른 작업을 수행하지 않고 대기 상태에 있게 된다.
* 예를 들어, 프로그램이 디스크에서 파일을 읽을 때, 동기 입출력을 사용하면 읽기 작업이 완전히 끝나고 데이터가 메모리에 저장된 후에야 다음 코드로 넘어갈 수 있다.
* 장점은 프로그래밍이 간단하다는 것이며, 입출력 작업의 완료를 쉽게 예측할 수 있다.
* 그러나 동시에 많은 입출력 요청을 처리해야 하는 프로그램에서는 비효율적일 수 있다.
* 동기 입출력 시스템에서는 입출력 작업이 프로세스의 실행을 막는 병목 현상이 발생할 수 있어, 시스템 자원이 충분히 활용되지 않는 상황이 발생할 수 있다.
* 따라서 대규모 시스템이나 멀티태스킹이 중요한 환경에서는 비동기 입출력(Asynchronous I/O) 방식이 종종 선호된다.

## 참고
- https://www.youtube.com/watch?v=mb-QHxVfmcs&list=PLcXyemr8ZeoQOtSUjwaer0VMJSMfa-9G-&index=13&pp=iAQB

# SpringPractice

## 🚀 동시성 이슈
### 🔍 동시성 이슈란 ?
여러 스레드가 동시에 같은 인스턴스의 필드 값을 변경 하면서 발생하는 문제를 의미함
### 💻 예방법
여러 클라이언트가 하나의 같은 객체 인스턴스를 공유하기 때문에 싱글톤 객체는 상태를 유지하게 설계하면 안됨
### 🎱 구체적인 나쁜 예시
* 특정 클라이언트에 의존적인 필드가 있으면 안됨
* 특정 클라이언트가 값을 변경할 수 있는 필드가 있으면 안됨
* 가급적 읽기만 가능해야 함
* 필드 대신 자바에서 공유되지 않는 지역변수, 파라미터, ThreadLocal등을 사용해야 한다.

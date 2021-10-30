## 1. 문제(Problem)

Spring 프로젝트를 개발하던 중 아래와 같은 메시지가 나타나고 메일전송 관련 작업에 에러가 발생하는 않는 현상이 발생했다.

      java.lang.NoClassDefFoundError: javax/mail/MessagingException


------------------

## 2. 해결(Solved)

####   - WEB/INF/lib 경로에 사용할 Mail 라이브러리 jar 파일을 넣어주면 된다.

![image](https://user-images.githubusercontent.com/54324782/139518809-49d9fa18-6ed1-4a16-987c-baabe94e9477.png)

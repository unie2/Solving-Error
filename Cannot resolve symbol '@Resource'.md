## 1. 문제(Problem)
  - Spring 프로젝트 진행 중 컨트롤러 파일에 @Resource를 작성하였지만, 아래와 같은 문구가 나타나면서 에러 표시가 났다.     

        Cannot resolve symbol 'Resource'

  ![image](https://user-images.githubusercontent.com/54324782/163737052-15a2e99c-42b5-4197-93e7-414fea1281e5.png)


------------------


## 2. 원인(Cause)

해당 라이브러리가 JavaEE Module인 java.xml.ws.annotation의 일부인데, java.xml.ws.annotation은 Java 9 부터 Deprecated 되었기 떄문이다.

------------------


## 3. 해결(Solved)

####   - pom.xml 파일에 아래와 같이 종속성을 추가해준 뒤 import 처리 해줌으로써 해결이 가능하다.

```xml
<dependency>
  <groupId>javax.annotation</groupId>
  <artifactId>javax.annotation-api</artifactId>
  <version>1.3.2</version>
</dependency>
```

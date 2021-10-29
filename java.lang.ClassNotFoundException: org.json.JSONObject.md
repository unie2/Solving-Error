## 1. 문제(Problem)

Spring을 이용하여 프로젝트를 개발하던 중 아래와 같은 메시지가 나타나고 JSON 관련 작업이 작동하지 않는 현상이 발생했다.

      java.lang.ClassNotFoundException: org.json.JSONObject

  
------------------

## 2. 해결(Solved)

####   - WEB-INF/lib 경로에 사용할 json 라이브러리 jar 파일을 넣어주면 된다.


![image](https://user-images.githubusercontent.com/54324782/139391042-3516cb18-d526-4dbd-b4e7-d2372dd4798e.png)

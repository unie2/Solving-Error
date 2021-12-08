## 1. 문제(Problem)

명령 프롬프트에서 mvn 명령어 사용이 안되는 현상이 있었다.

  

------------------


## 2. 해결(Solved)

####   - MAVEN 환경변수를 설정해주면 mvn 명령어를 사용할 수 있다.

내 PC > 오른쪽 마우스 클릭 > 속성 > 좌측 리스트 중 고급 시스템 설정 클릭 > 고급 > 환경 변수 > 시스템 변수 > 새로 만들기

![image](https://user-images.githubusercontent.com/54324782/145126179-e637dede-6ca2-49e3-aca1-b8adb68e2977.png)

그후 Path 항목에 아래와 같이 %MAVEN_HOME%\bin  을 추가해주면 된다.

다시 명령 프롬프트에서 mvn -v 를 입력하면 maven 버전을 확인할 수 있다.


## 1. 문제(Problem)

Spring을 이용하여 프로젝트를 개발하던 중 로그창에 나타나는 한글이 깨져서 이상하게 보이는 현상이 있었다.

  

------------------



## 2. 해결(Solved)

####   - 상단 우측 서버설정 부분 > Edit Configurations...

![image](https://user-images.githubusercontent.com/54324782/142146820-ac80bcc7-9ed3-4b96-8e95-a90c517501ee.png)


####   - VM options 항목에 " -Duser.language=en -Duser.region=us " 를 작성 및 저장한 뒤 서버 재시작 후 확인해보면 해결된다.

![image](https://user-images.githubusercontent.com/54324782/142146871-aa7b0c05-507a-4bfe-b3a2-8b9de06bc74b.png)

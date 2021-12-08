## 1. 문제(Problem)

SpringBoot & React 개발을 마무리하고 서버 배포 시 백엔드 단인 SpringBoot를 톰캣 서버에 먼저 배포했다.

그 후 프론트엔드 (React) 프로젝트를 배포 시 화면은 잘 나타나지만, 로그인 기능이 수행되지 않았다.

또한, "Invalid CORS request" 에러가 발생하였다.

------------------


## 3. 해결(Solved)

####   - 백엔드(SpringBoot) 프로젝트 내 Web관련 클래스에서 코드를 아래와 같이 수정하여, 접근이 가능해지도록 한다.

![image](https://user-images.githubusercontent.com/54324782/145125786-53fb6dea-34d7-4ec2-afcb-a0f3cc34cd21.png)



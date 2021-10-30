## 1. 문제(Problem)

Spring 프로젝트를 개발하던 중 아래와 같은 메시지가 나타나고 javax.mail 관련 작업에 에러가 발생하는 현상이 발생했다.

      javax.mail.AuthenticationFailedException: 535-5.7.8 Username and Password not accepted. ~
      

------------------

## 2. 해결(Solved)

####   - 첫번째로 javax.mail을 통해 gmail SMTP를 사용하기 위한 아이디 및 비밀번호 설정을 확인한다.

#####   아이디와 비밀번호 모두 오타없이 잘 작성되어 있어도 같은 오류가 발생한다면 아래와 같이 해결한다.

#### 1. 구글 계정에 로그인한 후 Google 계정 관리 항목에 접속한다.

#### 2. 보안 항목에 접속하여 "보안 수준이 낮은 앱의 액세스"를 확인한다.

#### 3. "사용 안함"으로 설정되어 있으면 "사용 함"으로 변경한다.


![image](https://user-images.githubusercontent.com/54324782/139518879-121ad4a9-8083-47cd-bef2-548067134af4.png)

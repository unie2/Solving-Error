## 1. 문제(Problem)
  - Android Studio Kotlin 언어로 개발 시 아래와 같은 에러 표시와 문구가 나타났다.

    ![문제](https://user-images.githubusercontent.com/54324782/155039139-4175630f-e0be-44fb-9186-346f07418ade.png)    

        Unresolved reference: ~
  

------------------


## 2. 원인(Cause)

레이아웃에 있는 요소 id를 참조하려면 kotlin-android-extensions 라이브러리를 사용해야 하는데 import 되어 있지 않았기 때문이다.


------------------


## 3. 해결(Solved)

![gradle(:app)](https://user-images.githubusercontent.com/54324782/155039317-7fac2eb5-cee0-4480-b2b8-d6f1c4d7f712.png)
#### (1) build.gradle(Module:project.app)에서 {id 'kotlin-android-extensions'}를 추가한다.

#### (2) 작성을 완료하면 Sync Now를 클릭하여 업데이트를 진행한다.
![import](https://user-images.githubusercontent.com/54324782/155039372-5e580e65-3f49-4d8e-94ef-893035cbc470.png)

#### (3) 문제가 되는 코드에서 Alt+Enter 혹은 import 버튼을 클릭하여 라이브러리를 Import 시켜준다.

#### (4) 아래와 같이 빨간 표시가 사라지면서 문제를 해결할 수 있으며, 애니메이터 실행 또한 잘되는 것을 확인할 수 있다.
![해결](https://user-images.githubusercontent.com/54324782/155039435-1674a29f-ad6c-4096-aece-ae3800a7f015.png)


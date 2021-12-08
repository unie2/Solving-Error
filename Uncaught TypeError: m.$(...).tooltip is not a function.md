## 1. 문제(Problem)

Summernote 라이브러리를 사용중인 React 프로젝트 실행 시 해당 페이지가 흰 화면으로 나오고 아래와 같은 에러가 발생했다.

![image](https://user-images.githubusercontent.com/54324782/145125924-74529fca-77d5-44ac-a663-0ec3113d3a78.png)


  

------------------


## 2. 원인(Cause)

사용 중인 react-summernote를 정상적으로 불러오지 못해 발생한다.


------------------


## 3. 해결(Solved)

####   - index.js 파일에 아래와 같이 코드 3줄을 추가하면 해결할 수 있으며, 정상적으로 페이지 접속이 가능해지고 오류가 사라짐을 확인할 수 있다.

![image](https://user-images.githubusercontent.com/54324782/145125988-d080a2ef-d8a1-40eb-a764-ad60f3318fc8.png)



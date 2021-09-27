## 1. 문제(Problem)

OpenCV를 이용하여 프로젝트를 개발하던 중 아래와 같은 에러 메시지가 나타났다.

      AttributeError: module 'cv2.cv2' has no attribute 'face'
  
원인은 'face'를 사용하기 위한 모듈이 프로젝트 내에 없기 때문이다.

  

------------------

## 2. 해결(Solved)

####   - 터미널에 아래와 같이 작성하여 해당 모듈을 설치하면 된다.

    pip install opencv-contrib-python
  


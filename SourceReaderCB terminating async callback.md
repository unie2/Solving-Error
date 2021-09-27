## 1. 문제(Problem)

OpenCV를 이용하여 프로젝트를 개발하던 중 아래와 같은 에러 메시지가 나타나고 카메라 영상이 나타나지 않는 현상이 발생했다.

      [ WARN:0] global C:\projects\opencv-python\opencv\modules\videoio\src\cap_msmf.cpp (674) 
      SourceReaderCB::~SourceReaderCB terminating async callback
  

  

------------------

## 2. 해결(Solved)

      cam = cv2.VideoCapture(0)

위와 같은 기존 소스코드에서 아래와 같이 카메라 영상을 활성화시키는 메소드 매개변수에 카메라 처리 API를 지정해준다.

      cam = cv2.VideoCapture(0, cv2.CAP_DSHOW)
  
두번째 매개변수에 해당하는 CAP_DSHOW는 카메라 영상이 화면에 바로 나타날 수 있도록 도와준다.

  
------------------

## 3. 추가 정보(Additional Information)  

 - PIL 이란?

아래는 주요 VideoCaptureAPIs 열거형 상수이다.

  1. CAP_ANY : 자동 선택  

  2. CAP_V4L, CAP_V4L2 : V4L/V4L2(리눅스)  

  3. CAP_FIREWIRE, CAP_FIREWARE, CAP_IEEE1394 : IEEE 1394 드라이버  

  4. CAP_DSHOW : 다이렉트쇼(DirectShow)  

  5. CAP_PVAPI : PvAPI, Prosilica GigE SDK  

  6. CAP_OPENNI : OpenNI  

  7. CAP_MSMF : 마이크로소프트 미디어 파운데이션 (Microsoft Media Foundation)  
  8. CAP_GSTREAMER : GStreamer  

  9. CAP_FFMPEG : FFMPEG 라이브러리  

  10. CAPIMAGES : OpenCV에서 지원하는 일련의 영상 파일 (예) img%02d.jpg  

  11. CAP_OPENCV_MJPEG : OpenCV에 내장된 MotionJPEG 코덱  


[추가정보 출처](https://thebook.io/006939/ch04/01/01-03/)

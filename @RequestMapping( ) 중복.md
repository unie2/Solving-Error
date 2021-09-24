## 1. 문제(Problem)

    Caused by: java.lang.IllegalStateException: Ambiguous mapping. Cannot map 'boardController' method
    .
    .
    .
    There is already 'boardController' bean method

  

------------------


## 2. 원인(Cause)

RequestMapping( )은 기본적으로 중복 값을 설정할 수 없다.

위 오류 메시지에 대한 원인은 RequestMapping( ) 매개변수 값을 중복하여 작성하였기 때문에 발생한 에러이다.

즉, 아래와 같이 @RequestMapping("/create-board")와 매핑 시 처리할 코드가 작성되어 있는데

![image](https://user-images.githubusercontent.com/54324782/134615165-744a6a0f-3b62-418b-b392-304cee315494.png)

처리 내용이 다르더라도 @RequestMapping("/create-board")와 같이 매핑 주소가 같은 코드를 또 작성하였기 때문이다.


------------------


## 3. 해결(Solved)

####   - 기존 매핑이 이루어진 코드에서 처리하거나 매핑 값이 중복되지 않도록 다른 값으로 설정하여 수행한다.

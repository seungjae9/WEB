# HTTP 프로토콜
### HTTP 프로토콜?

##### 프로토콜(Protocol)
* 컴퓨터나 원거리 통신 장비 사이에서 메시지를 주고 받는 `양식과 규칙 체계`

##### HTTP(Hypertext Transfer Protocol)
* 인터넷상에서 데이터를 주고 받기 위한 서버/클라이언트 모델을 따르는 프로토콜
* 어떤 종류의 데이터든지 전송가능(문서, 이미지, 동영상, 오디오 등)



##### 특징

1. stateless





### Methods

* 클라이언트가 웹 서버에 사용자의 목적/종류를 알리는 수단

  

1. GET
   * 파라미터를 넘겨 해당하는 Body를 받는다.
   * 오직 데이터를 받기만 한다.
2. HEAD
   * GET과 동일하지만 서버에서 Body(본문)를 Return 받지 않는다.
   * 응답의 상태 코드 확인
3. POST
   * 내용 전송(파일 전송 가능) - Sever에 Input Data 전송
   * 클라이언트에서 서버로 전달하고자하는 정보를 서버로 보낸다.
   * GET방식과 다르게 주소창에 보이지 않고 숨겨서 보낸다.
   * POST URL 은 Method 그 자체이며 페이지가 없다.
4. PUT
5. Delete





![img](https://t1.daumcdn.net/cfile/tistory/9935CE375AE7330A15)







### Status Code

* 1xx: 정보전달: 요청을 받았고, 작업을 진행 중이라는 의미
* 2xx: 성공: 작업을 성공적으로 받았고, 이해했으며, 받아들여졌다.
* 3xx: 리다이렉션: 요청을 완료하기 위해서 리다이렉션이 이루어져야 한다는 의미
* 4xx: 클라이언트 오류: 요청이 올바르지 않다는 의미
* 5xx: 서버오류: 올바른 요청에 대해 서버가 응답할 수 없다는 의미

##### 자주쓰는 Status Code
* 200 OK: 요청이 정상적으로 완료
* 400 Bad Request(잘못된 요청): 요청 자체가 잘못되었을때 사용하는 코드
* 401 Unauthorized(권한 없음): 인증이 필요한 리소스에 인증 없이 접근할 경우 발생
* 403 Forbidden(거부됨): 서버가 요청을 거부할 때 발생
* 404 Not Found(찾을 수 없음): 찾는 리소스가 없다
* 500 Internal Sever Error(내부 서버 에러): 서버에 오류가 발생해 작업을 수행할 수 없을 때 발생
* 503 Service Temporarily Unavailable: 일시적으로 서비스를 이용할 수 없을 때 발생


![ex_screenshot](./image/HTTPCODE.PNG)







https://shlee0882.tistory.com/107
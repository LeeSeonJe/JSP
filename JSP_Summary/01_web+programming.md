# 웹 ?
### 웹프로그래밍이란?
+ 웹프로그래밍이란, 웹어플리케이션을 구현하는 행위이다.
+ 웹어플리케이션이란, 웹을 기반으로 작동되는 프로그램이다.
+ 웹이란, 1개 이상의 사이트가 연결되어있는 인터넷 서비스의 한가지 형태를 말한다.
+ 인터넷이란, 1개 이상의 네이트워가 연결되어 있는 형태를 말한다.

``` 
http://wwww.sba.seoul.kr:80/kr/index
----   ----------------- -- ---------
  1           2,3         4    5
```
+ 1\. 프로토콜(Protocol) : 네트워크상에서 약속한 통신규약 (Http, FTP, SMTP, POP, DHCP)
  + (SMTP - 메일을 보내는 통신규약, POP - 메일을 받는 통신규약, DHCP - 동적 호스트 구성 프로토콜)
+ 2\. IP : 네트워크상에서 식별할 수 있는 주소
+ 3\. DNS : IP주소를 인간이 쉽게 외우도록 맵핑한 문자열
+ 4\. Port : 해당 컴퓨터의 구동되고 있는 프로그램을 구분할 수 있는 번호
+ 5\. informatiln path

### 웹프로그램의 동작
+ 웹서버
  + 클라이언트의 요청에 의해 정보를 제공해 주는 서버(Aphach, IIS),  
  별도의 구현이 필요한 로직이 있을 경우 웹어플리케이션 서버에 요청
+ 웹브라우저
  + 웹서버에 정보를 요청하고, 웹서버로부터 정보를 받는 매개체, 이때 HTTP 프로토콜을 사용함.

<br>

```
          > request          > Logic 요청                     > DB 접근
브라우저               웹서버               웹어플리케이션 서버             데이터베이스
          < response         < Logic 수행                     < 데이터
```
<br>

### 개발환경
이클립스 + 아파치 톰캣

+ 서버환경설정

![image](https://user-images.githubusercontent.com/59919620/76163205-83ec4480-6187-11ea-89be-118ce4df751d.png)

+ Server Location
  + Use Tomcat installation
+ Server Option 
  + Publish module contexts to separate XML files
+ Port
  + HTTP/1.1 변경 : 오라클 서버 내부적 http 프로토콜을 8080 사용하여 충돌 방지를 위해서 변경해준다.

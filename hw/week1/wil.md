#이번주에 배운 내용

1.WEB
2.클라이언트-서버
3.HTTP
4.프론트엔드 -백엔드
5.API

##1.WEB
웹이란 여러 컴퓨터가 서로 연결되어 정보를 공유하는 공간이다.

##2.클라이언트-서버
요청을 보내는 클라이언트와 요청을 수행하는 서버 가 있다.
클라이언트와 서버는 역할의 개념이지 기계의 개념은 아니다.

클라이언트는 데이터의 생성/조회/수정/삭제 요청을 전송한다.
서버는 요청대로 동작을 수행하고 응답을 전송한다.(실패했음 이라는 응답을 하기도함)

##3.HTTP
HTTP는 웹에서 사용하는 프로토콜이다.
프로토콜은 네트워크 내부에서 요청과 응답을 보내는 규칙이다.

HTTP를 통해 요청을 보낼 땐 HTTP Method 와 URL이 필요하다.

HTTP Method: 데이터를 다루는 방법을 의미한다.
URL(Uniform Resource Location): 다룰 데이터의 위치를 표현한다.

자주사용하는 HTTP Method

1.GET: 데이터를 가져온다
2.POST: 데이터를 게시한다.
3.PUT: 데이터를 교체한다.
4.PATCH: 데이터를 수정한다.
5.DELETE: 데이터를 삭제한다.

##4.프론트엔드와 백엔드

자주변하지 않는 화면 UI 와 컨텐츠를 분리한다.
여기서 UI는 대부분 프론트 엔드에서 구현하며 컨텐츠는 백엔드에서 구현한다

프론트는 화면에 채울 컨텐츠 데이터를 백엔드에게 요청하여 화면에 렌더링하는 작업을 한다.
백엔드는 DB에서 가져온 컨텐츠 데이터를 프론트에게 보내준다(대부분 JSON 형태로 데이터를 받음)

##5.API(Application Programing Interface)

어플리케이션에서 원하는 기능을 수행하기 위해 
##어플리케이션과 소통하는 구체적인 방법을 정의한 것
어플리케이션의 사용설명서 이다.

백엔드 API

프론트가 백엔드에 요청을 보낼 때
어떤 http method, url을 사용해야 하는지 정의한 것
각 요청에 대해 어떤 응답을 보내는지 정의한것

REST API
REST 아키텍처를 따르도록 설계한 API
URL은 조작할 데이터를 나타낸다.
HTTP method는 데이터에 대한 행위를 나타낸다.


#API 명세서

##1.할 일 관리 API
1.할 일 생성: POST/todo
2.할 일 조회: GET/todo/list
3.할 일 수정: PATCH/todo/{todo_id}
4.할 일 삭제: DELETE/todo/{todo_id}
5.할 일 체크: PATCH/todo/{todo_id}/check
5.할 일 체크해제:PATCH/todo/{todo_id}/uncheck

##2.유저 관리 API
1.회원가입(회원 정보 생성): POST/signup
2.로그인(회원 정보 확인): GET/login
3.로그인 성공: GET/userInformation

##3. 친구 API
1.친구 추가: POST/USER/{user_id}
2.친구 조회: GET/myFreinds
3.친구 삭제: DELETE/myFreidns/{user_id}
4.특정 친구의 할 일 조회:GET/USER/{user_id}



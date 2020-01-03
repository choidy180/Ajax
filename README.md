# 2.1Ajax

Ajax란 HMLHttpRequest라는 스크립트의 객체를 이용하여 웹 서버와 비동기로 통신하고 DOM을 이용하여 웹 페이지를 동적으로 갱신하는
프로그래밍 비법을 말한다 Ajax의 기술은 2005년 등장한 이후 급속히 보급되었으며 클라이언트 측 자바스크립트의 필수적인 기술이 되었다

# 2.2 Ajax의 특징

Ajax를 활용한 웹 어플리케이션으로는 구글 지도(Google Maps), 네이버 지도 등의 지도 서비스가 있습니다. 네이버 지도 서비스를 이용하여
기존에 사용하던 기법과 Ajax 기법이 어떻게 다른지 보본다

+ 기존의 지도 서비스

사용자가 찾아보려는 장소가 바뀌면 클라이언트는 서버에 새로운 지도 정보를 보내 달라는 요청을 보낸다.
서버는 이 요청을 받아서 새로운 지도를 포함한 웹 페이지 전체를 생성한 후에 클라이언트로 전송한다.
클라이언트는 이 결과를 받아 웹페이지 전체를 다시 렌더링 해서 표시한다. 이때 일련의 통신은 동기적으로 이루어 진다
따라서 서버가 모든 데이터를 보내기 전까지 클라이언트는 아무것도 할 수 없는 상태가 된다. 또한 웹 페이지 전체를 주고받아야 하기 때문에
그만큼 시간이 걸린다

+ Ajax를 활용한 지도 서비스

사용자가 찾아보려는 장소가 바뀌면 클라이언트 측 자바스크립트가 현재 가지고 있는 지도 데이터에서 부족한 부분을 파악한다
그리고 서버에 그 부분만 보내달라는 요청을 보내고 이 요청을 받은 서버는 클라이언트가 필요로 하는 데이터만 전송한다
클라이언트는 이 데이터를 받아서 필요한 부분만 DOM으로 변경, 이때 일련의 통신은 비동기적으로 이루어지고 따라서 서버가
데이터를 다 보내지 않은 상태라도 클라이언트를 자유롭게 사용할 수 있다.

# Ajax의 장점

+ 최소한의 데이터 통신만 하므로 처리속도가 빠르고 서버 부화와 통신트래픽 부하가 적다
+ 비동기로 통신하므로 클라이언트 측에서 다른 작업을 할 수 있다
+ 웹 페이지 갱신을 클라이언트 측이 담당한다. 페이지를 전환하는 대신에 페이지 일부분만 변경하므로 고속 랜더링이 가능하다


Ajax를 활용하면 화면을 전환하는 빈도가 줄어들어 사용자에게 데스크톱 애플리케이션을 사용하는 듯한 편의성을 제공할 수 있다


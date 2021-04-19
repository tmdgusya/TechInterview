# MPA (Multiple Page Application)

- 가장 전통적으로 이용되는 방식 중 하나이다, **모든 페이지가 각각의 html 로 이루어지는 (Multiple) 방식**이다.

- 즉 하나의 페이지에서 다른 페이지로 이동하기 위해서는 **반드시 Request 를 보내고 원하는 페이지의 Response 를 받아야 함**을 의미한다.
  이러한 방식은 한가지 단점이 있을 수 있는데 단점은 아래와 같다.

- 페이지가 바뀔 때 마다 매번 완전한 페이지를 응답으로 받는다. => 필요한 부분만 응답 받는 방식에 비해 비효율적이다
- 페이지가 바뀔 때 마다 브라우저가 잠시 Reload 되는 단점이 있다 => Client 입장에서는 좋지 않음

# SPA (Single Page Application)

- **SinglePageApplication** 은 위와 반대로 생각하면, **초기에 시작될때 모든 데이터를 다 받아오는 것**이다.
  즉 하나의 Page 로서 운용되는 것이다. 그래서 **초기 페이지 로딩이 오래 걸린다는 단점**이 있다.
  그리고 페이지가 전환될때 프론트 서버에 Request 를 보내는 것이 아니라, 클라이언트 자체에서 JS 에 의해 전환된다.
  페이지내에 동적으로 변해야 하는 부분이 있을 경우 해당 정보만 백엔드 서버에 요청하여 응답을 받고 웹에 갱신하는 방식이다.
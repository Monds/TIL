NodeJs 정확한 이해.


Node는 구글 크롬의 V8 자바스크립트 엔진 기반으로 만들어진 서버사이드 플랫폼.
사용 언어는 자바스크립트

이벤트 기반

논블록킹 I/O 모델 (비동기)
모든 API가 비동기 처리.
결과 전달은 이벤트 매커니즘으로 나중에 전달됨.

apache 와 nginx(node) 웹서버 비교
https://victorydntmd.tistory.com/231

npm 생태계는 매우 커서 별도 웹 어플리케이션 서버 없이 nodejs 만으로 운영이 가능하나
직접 모든 환경을 구성하는 것은 어렵기에 express, koa, hapi 같은 웹 프레임워크를 선택한다.


** 웹서버: 정적 컨텐츠
** WAS(Web Application Server) : 동적 컨텐츠

톰캣같은 WAS를 사용하면 .. 단독으로 사용가능하지만 (톰캣이 웹서버의 기능을 포함하고 있기 때문)
보통 로드밸런싱을 해주러면 apache나 nginx를 사용해야 한다.
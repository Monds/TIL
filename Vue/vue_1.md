### export
Javascript 모듈에서 함수, 객체, 원시 값을 내보낼 때 사용.
내보낸 값은 다른 프로그램에서 import 문으로 가져가 쓸 수 있다.

기본적으로 named, default export가 있다.

default로 export할 경우 괄호를 사용하지 않아도 import가 가능

### Virtual DOM
양방향 바인딩을 통한 모델(M)과 뷰(V)의 데이터 변화
Virtual DOM을 이용한 DOM 변화 최적화
(React, Vue에서 사용)


### Vue 인스턴스 기본 속성
- name: (컴포넌트 옵션에서 사용) 

디버깅에 이점. 
* vue-devtools 에서 익명의 컴포넌트는 <AnonymousComponent>
로 표시됨.

- data: 데이터 객체 **데이터의 모든 속성을 프록시 처리함.
dom에 데이터 랜더링.
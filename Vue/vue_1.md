## Virtual DOM
양방향 바인딩을 통한 모델(M)과 뷰(V)의 데이터 변화
Virtual DOM을 이용한 DOM 변화 최적화
(React, Vue에서 사용)


## Vue 인스턴스 기본 속성
- name: (컴포넌트 옵션에서 사용) 

디버깅에 이점. 
* vue-devtools 에서 익명의 컴포넌트는 <AnonymousComponent>
로 표시됨.

- data: 데이터 객체 **데이터의 모든 속성을 프록시 처리함.
dom에 데이터 랜더링.

## import ... from 시의 @의미
resolve alias 로 '@'이 root의 src폴더로 링크되어 있다.
https://stackoverflow.com/questions/42749973/es6-import-using-at-sign-in-path-in-a-vue-js-project-using-webpack


## 플러그인 사용
Vue.use 의 global 메서드를 사용하여 플러그인을 사용할 수 있다.

Vue.use(Vuex)
Vue.use(Router)
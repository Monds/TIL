## Webpack
웹 어플리케이션 구동을 위해 필요한 모든 모듈을 하나의 파일로 묶어 패키징해준다.
(모듈 번들러)

head에 선언하는 전통적인 방식으로는 자바스크립트 파일을 관리하기 어렵다.
선언되는 순서도 신경써야 하고, 전역 변수를 재사용하는 위험도 존재한다.
중복된 소스도 많아지고 global 이 복잡해진다.

이를 webpack이 하나의 파일로 번들링하여 해결해준다.

## babel 
최신 자바스크립트 문법 trans compiler 
최신 문법은 브라우저에서 지원을 하지 않는 경우가 많다.
최신 문법을 사용하여 생산성을 높이고 babel로 브라우저 호환에 맞춰 변환한다.


## JSX
html 이 아니고 자바스크립트.
UI 를 렌더링하기 위한 template language

## Props & State
props 는 부모 component가 자식 component에 전달하는 값. (수정 불가능)
state는 component 내부에서 사용하며 값 변경 가능

**보통 관리하는 state가 없고 LifeCycle API를 사용하지 않을때에는 functional component를 사용한다.**

## Middleware

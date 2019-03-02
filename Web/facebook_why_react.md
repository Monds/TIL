# FBDG 2015 Nov - Facebook, React 정리

## UI에서의 State
상태의 의미는 다음과 같다.
>현상이 놓여있는 모양이나 형편

이를 대입해보면 웹에서는 UI가 놓여있는 모양이나 형편으로 볼 수 있는데<br>
우리가 보는 UI는 특정 시점의 데이터를 표현한다. <br>
즉 상태관리는 곧 데이터 관리로 볼 수 있다.

## jQuery
jQuery로 DOM Selecting이 쉬워지고 브라우저 호환 등의 장점으로 dynamic한 페이지를 만들 수 있었지만 기능이 많아짐에 따라 소스의 복잡도가 올라갔다.

- 유지보수 어려움
- 잦은 DOM Selecting 으로 인한 성능 저하
- 코드 유연성 저하 (HTML, Javascript, CSS의 결합)
- 테스트 곤란
- 관심사 분리, OOP 관점의 설계가 없다.

## MVC
웹프론트엔드에 MVC 적용이 시작됨. <br>
backbone.js 가 등장하였는데 model, view의 관점이 생겼으나
결국 model에서 view(js)에서 이벤트를 받아 상태(HTML)에 변경해주는 부분은 아직 개발자가 모두 구현을 해야함.
** event만 notify해주는 observer로 보면 된다.

## 양방향 데이터 바인딩
view에 데이터를 html에 바인딩하는 부분을 프레임워크가 처리<br>
angular, react
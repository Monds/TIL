# MVVM
Model - View - ViewModel 패턴<br>
WPF, SilverLight 등에서도 많이 쓰는 패턴

MVC모델과 비교하였을 때 기존에 모델이 변경되었을 경우에는 뷰는 컨트롤러를 통해서 통보를 받았다.<br>
컨트롤러가 ViewModel로 교체가 된 형태고 뷰가 필요하는 데이터와 액션을 담고 있는 컨테이너 객체로 보면 된다.

다음 2가지 특징으로 기존 controller의 역할을 대체할 수 있게 된 것이다.
- command pattern
- data binding

## Commmand Pattern
실행될 기능을 캡슐화하는 패턴
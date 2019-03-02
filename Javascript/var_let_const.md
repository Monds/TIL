## 차이점 정리
|| var | let | const |
|-| :---: | :---: | :-----: |
|재선언 (redeclare)|가능|불가능|불가능|
|재할당 (reassigned)|가능|가능|일부가능*|
|선언 전 사용|가능|불가능|불가능|
|Scope*|Function|Block|Block|

>const는 참조형(array, object, function)의 경우 수정이 가능하다.


## TDZ (Temporal Dead Zone)
일시적 사각지대  
let, const는 var과는 달리 호이스팅되어도 TDZ가 생성되어 변수 선언 전까지 접근할 수 없다.



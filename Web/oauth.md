# OAuth
네이버 D2 에 올라온 글을 정리하였다.

## 개요
SaaS(Software as a service)
Facebook이나 트위터의 일부 기능(친구 목록을 가져온다는지 등등..)을 사용하기 위해 페이스북이나 트위터에 로그인을 해야하는 것 이 아닌 별도의 인증 절차를 거치면 다른 서비스에서 쉽게 이용할 수 있게 했다.

이때 사용하는 인증 절차가 OAuth

## OAuth
> 인증을 위한 오픈 스탠다드 프로토콜  
> 타사의 API를 사용하고 싶을 때 권한 획득을 위한 프로토콜

현재 대부분의 유명한 인터넷 서비스 기업은 모두 OAuth를 사용하고 있다.

> OpenID 도 인증을 위한 프로토콜이지만 다르다.

인증(Authentication) 과 권한부여(Authorization)을 함께 진행한다.
사용자의 아이디와 암호가 노출되지 않으면서 API 접근 위임이 가능한 방법.

Open Authentication, Open Authorization

## OAuth 1.0 과 2.0의 차이
사용용어가 다르고
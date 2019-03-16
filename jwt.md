## JWT (Json Web Token)

웹표준.
access token

## 세션 기반 인증의 문제점
데이터베이스에서 관리 시 성능에 이슈
메모리도 한계가 있음
서버 확장이어려움(스케일아웃)



# 회원인증
1. 사용자가 로그인을 하면 서버는 유저의 정보에 기반한 토큰을 발행하여 유저에게 전달
2. 유저가 서버에 요청할 때마다 JWT를 포함하여 전달
3. 서버는 요청을 받을 때마다 토큰이 유효하고 인증되었는지 검증을 하고 권한을 체크하여 작업 처리

# 장점
1. 유저의 session을 유지할 필요가 없음 (stateful)
2. Scale out 고려시 세션 클러스터링 로드밸런싱을 고려하지 않아도 됨 - 클라우드 환경에 유리

# 단점
1. 길이. 호출할때마다 헤더에 붙여서 보내야 해서 네트워크 대역폭 낭비가 심함
2. 토큰 내부 정보 유출의 위험. --> 토큰 자체를 암호화하는 방법이 있음.

## 구조
header / payload / signature

## Header
typ: JWT
alg: Hasing 알고리즘 (RSA, HMAC SHA256)

## Payload
** 클레임(claim): 정보의 한 조각. 사용자에 대한 프로퍼티나 속성
registered claim: 고정된 클레임. 토큰 발급자, 토큰 제목, 토큰 대상자, 만료시간
public claim: 충돌 방지를 위한 이름 (URL)
private claim: client 와 server간 협의하에 사용

## Signature
header와 payload를 base64 인코딩하여 . (dot) 으로 구분하여 붙힌 후 비밀키로 해쉬하여 생성
서버는 header와 payload를 signature와 비교하여 다르면 깨졌다고 판단함.


## 보안의 문제
일반적으로 oauth같은 경우 expire date를 5분 ~ 60분으로 짧게 가져감.
슈퍼컴퓨터를 활용하여도 깨지는 데 시간이 걸리기에 쉽지 않다.
물론 한시간내에 깰수 있으니 안전하지는 않다.
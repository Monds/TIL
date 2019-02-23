# IntelliJ 초기설정
## 윈도우10 DPI 변경 시 메뉴가 깨져보이는 현상 수정
vm option에 아래 항목 추가
`-Dsun.java2d.uiScale.enabled=false`

## Code Completion 대소문자 체크 해제
Editor > General > Code Completion 에서 Match case 체크 해제

## Console font size 변경
Editor > Color Schema > Console Font

## Method chaining enter tab indent
spring boot java config 코딩 시에 method chaining 을
여러 줄로 할때 엔터가 더 들어가는데
아래 설정으로 변경 시 잘 된다.
Editor > Code Style > Java > Tab and Indents 의 Continuation indent 값을 4로 변경

## Auto Import
Editor > General > Auto Import 에서
Add unambiguaous imports on the fly 체크

## 창 전환 시 code completion이 제대로 안될 때
source root를 mark as source를 해제했다가 다시 해본다.  
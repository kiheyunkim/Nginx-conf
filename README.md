# Nginx

## 참고 레퍼런스

http://nginx.org/en/docs/http/ngx_http_core_module.html

## 추가 설명

location [=|~|~*|^~|@] pattern { … }

* 패턴
  * =  : 패턴과 정확하게 일치
  * ~  : 정규표현식과 일치
  * ~* : 대소문자 구분 않고, 정규표현식과 일치
  * ^~ : 지정한 패턴으로 시작해야함.(패턴 일치시 다른 패턴 탐색 중지)
  * @  : 이름가진 location 블럭을 정의함. 내부 요청에 의해서만 접근 가능.
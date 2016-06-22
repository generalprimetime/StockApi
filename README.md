# StockApi
==========

COM (Component Object Model 방식)
=================================
CybosPlus (대신증권)
----------
* 전용 프로그램을 통한 로그인 (CYBOS5.exe) 
* API doc (CoBos plus) 
* 다양한 Class 제공 

[장점]
로그인을 전용 프로그램이 관리하여 개인정보가 안전 

[단점] 
 API로 로그인 불가,
 Callback함수가 없음 (정보를 얻기위해 매번 함수 호출) 

XingAPI(이베스트)
-----
* Event 형식의 return. Callback 형태로 동작
* 총 3개의 Class만 제공 
* API doc (DevCenter)

[장점] 
API로 로그인 가능 > 알고리즘 트레이딩 프로그램의 자동화 관점에서는 분명히 편리

[단점]
초보자들에게는 API를 이용한 로그인이라는 과정 자체가 큰 진입 장벽, 로그인정보 보안처리 로직이 필요할 수도 있음 

COX (Object Linking and Embedding Custom Control 방식)
===========
OpenAPI+(키움증권)
-------
* 키움증권에서 제공하는 GUI를 띄워 로그인을 요청해야함 
* API Doc (KOA Studio) 

[장점]
PyQt로 만들어지기 때문에 UI 구현이 따로 필요치 않음  

[단점]
COX방식은 COM에 비해 파이썬에서 사용하기가 쉽지 않음 > PyQt패키지의 QAxContainer 모듈을 통해 OCX를 사용함

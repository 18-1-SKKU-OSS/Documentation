서비스 관리자 디자인 패턴
===================

기본 개요
-------

인터넷을 통해 연결하는 모든 장치(클라우드) 또는 LAN 장치들은 정의된 서비스 관리자 SmartApp를 요구한다 또한 일반적으로 장치 핸들러가 요구 될 수도 있다.
서비스 관리자는 장치와 연결하여 입력 및 출력 상호 작용을 처리하고 장치 핸들러는 메시지를 구문 분석합니다(parse).

클라우드 연결 장치
--------------

클라우드로 연결된 장치를 사용할 때 서비스 관리자는 허브(Hub)를 검색하고 외부와의 OAuth 연결을 사용하여 허브와 연결합니다.
그런 다음 장치 핸들러는 이 연결을 통해 허브와 장치간에 통신합니다.

LAN연결 장치
----------

LAN연결 장치를 사용할 때 서비스 관리자는 허브(Hub)를 검색하고 SSDP나 mDNS/DNS-SD 프로토콜을 사용하여 허브와 연결합니다.
그런 다음 장치 핸들러는 UPnP/SOAP 호출 또는 REST 호출을 통해 허브와 장치간에 보내는 메시지를 통신합니다.

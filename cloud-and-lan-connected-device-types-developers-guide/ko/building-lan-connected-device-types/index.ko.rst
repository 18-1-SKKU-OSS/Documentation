LAN연결 장치 유형 만들
===================================

LAN연결 장치는 LAN을 통해 SmartThings Hub와 통신합니다.

그러한 장치의 예는 Sonos 시스템이다.

LAN장치용 장치 핸들러를 개발하는 경우 서비스 관리자를 생성해야 합니다.

LAN상의 장치 검색을 처리하는 SmartApp은 경우에 따라 장치와 통신하고 이벤트를 통해 발생하는 장치 변경에 대응합니다.

이 가이드에서는 ServiceManager. DeviceHandler아키텍처의 개념을 간략히 소개하고 ServiceManager및 DeviceHandler생성의 예를 제공합니다.

목차:

.. toctree::
   :maxdepth: 2

   division-of-labor
   building-the-service-manager
   building-the-device-type

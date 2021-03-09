AARRR
=============

## Retention

* Retention
  - Activation 과정을 통해서 경험한 A HA Moment를 꾸준히 경험하도록 하는 것
  - 서비스의 성공을 예측할 수 있는 가장 중요한 지표중 하나

* Retention을 측정하는 세가지 방법
  - Classic Retention
  - Range ""
  - Rolling ""

* Classic Retention(Day-N Retention)
  - 특정일에 come back한 유저의 비율
  - 각 날짜에 접속한 유저는 독립적으로 계산
  - 계산 : Day M에 서비스를 사용한 사람 / Day 0에 처음 서비스를 사용한 사람
  - 장점
    - 설명, 계산하기 쉽다
  - 단점
    - 특정일의 noisie에 매우 민감, 일 단위 로그인 데이터를 모두 쌓아둬야 함
  - 활용
    - Daily Use가 중요한 서비스(전화)
    - Noise를 줄이려면? 기준일을 여러 개 두고, 여러 번 측정해서 Day N 리텐션의 평균값을 활용



* Range Retention
  - 특정 **기간**에 come back한 유저의 비율
  - 기준을 개별 날짜가 아닌 특정 기간(주, 월)으로 한다
  - 각 기간에 접속한 유저는 독립적으로 계산됨
  - 계산 : Range N에 서비스를 사용한 사람 / Range 0에 처음 서비스를 사용한 사람
  - 장점
    + 설명이 쉬움, Day-to-Day Noise에서 자유로움
  - 장점
    + Range가 길어질수록 over-estiamte 
    + 의미있는 결과를 보기 위해서는 꽤 오랜 시간이 필요
  - 활용
    + Daily Use가 덜 중요한 서비스(가계부)  

* Rolling Retention
  - 몇 명이 남아있는가? 가 아니라, 몇 명이 나갔는가?에 초점을 맞춘 리텐션 계산
  - 계산 : After N day에 서비스를 쓴 기록이 있는 사람 / Day 0에 처음 서비스를 사용한 사람
  - 장점
    + 계산하기 쉬움, Retension의 기준을 임의의 기간으로 설정하지 않고, 온전히 사용자에게 맡김
  - 단점
    + 전반적으로 over-estimate
    + 아상치의 영향이 매우 큼  
    + 계속 변화하는 숫자
  - 활용
    + 자주 쓰이지 않는 서비스에서의 리텐션 측정

* Engagement = DAU(Daily Active User) / MAU(Montly Active User)
  - Engagement 비율을 통해, 사용자가 특정 서비스에 얼마나 engage 되었는지를 가늠
  - 단, Daily use가 전제된 서비스에서만 유효한 지표(전화, 문자, 카톡 등)
  - Retained유저와 그렇지 않은 유저를 나눠서, Drill-down하는 분석이 뒤따라야 함
  -  서비스 간 비교는 쉽지 않음
  -  동일 서비스에서의 기간별 추이를 보면 유용함

* Cohort
  - Funnel 분석과 마찬가지로, Retention도 Cohort를 쪼개서 차이를 보는게 핵심
  - 데이터를 들여다보면 Activation * Retention * Revenue는 자연스럽게 이어지는 과정

* Retention의 기준
  - Log-in이 **유의미한 행동**이기 때문에, 이를 시간에 따라 반복하는지 보는 것
  - 다른 유의미한 행동을 기준으로, 시간에 따른 반복을 보는 것도 괜찮음

* Retention 개선하기
  - 함정카드가 많은 영역 : 지표에 매몰되기 쉽다.
  - Key feature를 기준으로 리텐션 모니터링
  - 추적된 가치
  - 습관
  - 장기간의 리텐션이 중요하다는게 어려운 포인트
  - 일관되게 유지되지 않음
    + 기간에 따른 코호트분석을 해야하는 이유
  - 카테고리마다 권장되는 레텐션 수준이 다름 So 목표 수준을 잘 정의
  - 보통 AARRR에서 activation과 함께 가장 먼저 개선해야 하는 항목으로 꼽힘

##

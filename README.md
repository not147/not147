# LHK Portfolio_Project

## # master's thesis - 머신러닝을 이용한 지하매설물 탐사

* Background

  지하매설물의 노후화, 확인하기 어려움 때문에 보다 효율적인 탐지방법이 필요

  현재 나온 탐지방법들은 명확한 한계를 가지고 있음

  한계를 보완하기 위하여 머신러닝 알고리즘을 사용



- Summary

  (1) Data Collection

      Comsol multiphysics를 이용하여 모델링 후 가상 데이터 추출 (Comsol 데이터)

      현장에서 전기 비저항 방식으로 데이터 추출 (현장 데이터)

  
  

  (2) Data Preprocessing

      TDA (Topological Data Analysis) : 수치화된 데이터를 위상적 방법을 통해 시각 데이터로 보는 데이터 분석 기법

      Min_Max scale : 현장 데이터와 Comsol 데이터 간의 차이를 보완

      연속형 데이터 추가 : Comsol 데이터에 noise를 가해 데이터의 문제점 보완

  
  

  (3) Model & Algorithms

      Random Forest, XGBoost, SVM, RNN, CNN 등등 여러 알고리즘을 사용하여 정확도를 비교 (Regreesion 사용)

  
  

  (4) Review

      Comsol 데이터 만 사용했을 때는 정확도가 매우 낮았지만 현장 데이터가 추가된 시점에서는 정확도 상승

      현장 데이터의 비율이 매우 낮음

      실제 현장에서 시험한 결과 45개 case에서 43개 case가 오차범위 내에 들어옴

      현장 데이터의 수를 증가시키면 더욱 좋은 결과가 나올 것으로 보임

  

  보러가기 : 

  논문링크:  http://www.riss.kr/search/detail/DetailView.do?p_mat_type=be54d9b8bc7cdb09&control_no=cb1fd322c9f43100ffe0bdc3ef48d419
  
  

### #1. Project - FDS(이상거래탐지)

* Background

  이상거래탐지에 가장 주된 알고리즘은 규칙 기반(Rule-Based) 의 탐지방법

  이 데이터를 이용하여 데이터 분석 및 예측모델 생성하여 탐지방법 강화



* Summary

  (1) Data Collection

   은행 거래 데이터

  

  (2) Data Preprocessing

   TDA (Topological Data Analysis) : 수치화된 데이터를 위상적 방법을 통해 시각 데이터로 보는 데이터 분석 기법

   tSNE (t-Stochastic Neighbor Embedding) : 차원 축소 및 시각화 도구

  

  (3) Model & Algorithms

   Random Forest, XGBoost, SVM, RNN, CNN 등등 여러 알고리즘을 사용하여 정확도를 비교

  

  (4) Review

   정상거래에 비해 이상거래 데이터의 수가 매우적음

   중복 되는 경우가 많음 (거래정보는 똑같은데 입출금 금액만 다른 경우가 많음)

  

  보러가기 : 

  ​	

### #2. Project - 서울시 골목상권 매출과 코로나 확진자 수와의 관계

  

* Background

  코로나로 인해 상권들의 매출 타격이 컸는데 그 중 골목상권이 큰 타격을 입음

  다양한 방역정책이 나오고 있는 시점에서 매출과 코로나 확진자 수가 어떤 관련이 있는지 

    

* Summary

  (1) Data Collection

   19~20년 골목상권 매출 데이터

   20년 코로나 확진자 데이터

   19~20년 유동인구 데이터

  데이터 출처 : https://data.seoul.go.kr/

    

  (2) Data Preprocessing

   데이터 통합

    

  (3) Model & Algorithms

   상관 분석

   시각화

    

  (4) Review

   초창기 확진자 수가 적을 때는 매출에 큰 지역에서 상대적으로 코로나 확진자 수가 많아짐

   3~4분기에 오면서 확진자 수가 급증하였고 매출이 큰 지역보단 유동인구가 많은 지역에 코로나 확진자 수가 많아짐

   정부 방역정책의 목적은 거리두기이고 이 결과는 확진자 수가 많아 질 수록 유효한 방역정책으로 보임

   하지만 여전히 집단감염 비율, 고위험군 시설, 종교, 병원 시설의 감염 비율이 큰 비중을 차지함

    

  보러가기 :  https://not147.github.io/


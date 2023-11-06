# HD-AI-Challenge

## 최종 순위 (23.11.06. 기준)

### Kim & Hwang

|Public|Private|
|----|---|
|26 / 342|34 / 330|


## 대회 소개
https://dacon.io/competitions/official/236158/overview/description

## 특이점
1. Regression task임에도 불구하고 CI_HOUR(target)이 0인 비율이 40.12%이기 때문에 일차적으로 Classification을 통해 CI_HOUR가 0인지 아닌지 예측을 한 뒤 Regression을 통해 예측

2. 데이터의 분포가 Power-law distribution 형태를 띄었기 때문에 log scaling을 통해 보정

3. 유가 및 해상운임지수 데이터 추가

4. Volume, Load_Capacity 등 파생변수 생성

## 추가 시도 (성능 개선 X)

1. 절반 정도의 데이터에서 풍속, 기온 등이 결측치로 존재하였기 때문에 다양한 Imputing 방식을 시도

2. DateTime에 Cyclic_transform을 적용

## 향후 시도하면 좋을 것들

1. 하이퍼파라미터 최적화를 위한 라이브러리(Optuna)를 사용 
2. 배의 나이, 달러 환율과 같은 변수 추가
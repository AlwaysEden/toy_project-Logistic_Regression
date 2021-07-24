# toy_project-Logistic_Regression

## 1. 개발목적
Logistic Regression을 공부하고 이를 실제로 구현 해보기위한 학습적 목적으로 개발했음.

## 2. 설명
데이터셋은 케글의 Social_Network_Ads.csv 파일을 가져와 사용했음.
이 모델은 로지스틱 회귀 알고리즘을 이용해서 Purchased를 예측하는 이진분류 모델임. 

## 3. 개발일지
2021.07.23 데이터를 읽고 나누고 학습시켰지만 정확도가 0.5~0.6으로 많이 낮았음. 이 문제가 데이터 양의 부족으로 생각해 polynomialfeature을 통해 특성을 늘렸지만 오히려 역효과가 났음.

2021.07.24 다시 소스코드를 확인해본 결과 StandScale을 하지 않고 특성추출을 한 것을 발견했으며 이 문제를 해결하기 위해 StandScale을 했음. 이후 수정된 데이터를 가지고 fit하고 score을 확인해 본 결과 아주 만족스러운 결과를 얻었음. 이후 predict_proba와 sigmoid function을 통해 각 분류가 어떤 확률을 가지고 분류 되었는지 확인하는 작업까지 해봄

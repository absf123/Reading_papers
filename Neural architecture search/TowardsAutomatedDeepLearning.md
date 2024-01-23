### 240122
#### ICML'18 AutoML workshop
#### 요약
1. 기존 NAS는 hyperparameter tuning을 따로 분리되어 진행되었고, 이러한 분리는 suboptimal을 가져옴\
2. 그 이유는 two step으로 이뤄지는 architecture를 찾는 과정과 그 구조의 hyperparameter tuning 절대적인 epoch 차이로 인한 것\
⇒ 예를 들어 architecture를 찾는 과정은 20 epoch, hyperparameter tuning은 600 epoch으로 크게 차이 나는 경우 relatively ranking이 상관관계가 낮을 수 있다.\
⇒ 즉, 뒤에 있는 600 epoch의 훈련 시간이 의미가 없을 수 있음
3. 그래서 우리는 NAS를 categorical hyperparameter로 변환하고 이를 HP search space에 추가해 HPO 문제를 푸는 으로 casting하였고, BOHB를 이용해 이를 더욱 효과적으로 탐색을 했다.

#### 논문 소속: Frank Hutter [[Link]](https://ml.informatik.uni-freiburg.de/team/)

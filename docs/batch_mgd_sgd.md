# Batch, Mini-Batch, Stochastic
* epoch: 몇 번 학습할 것인지 나타내는 값
* batch: 한 번의 `epoch`에서 전체 트레이닝 셋을 돌면서 학습하는 것을 batch 라고 부른다.
* mini-batch: 한 번의 `epoch`에서 전체 트레이닝 셋에서 일정 부분만 떼어서 학습하는 것을 Mini-Batch라 한다.
    * Mini-Batch는 Over-fitting 문제를 해결하기 위해 이용한다.
* SGD: Stochastic Gradient Descent란 하나의 학습데이터만을 Backpropagtion을 진행함으로서 학습 성능을 높이는 것을 말한다. 이 방식은 Gradient Descent보다 Overfitting 발생 확률은 적지만 Global Minimum에 도달할 확률 또한 낮아진다.
    * Batch Size의 학습에서 MSE(Mean Squared Error)_Loss를 이용하면 전체 트레이닝 셋에 대한 오차를 구하기 때문에 계산량이 많아진다. 반면, SGD는 하나이 데이터 셋에서만 Loss를 구하고 이를 바로 역전파 시키기 때문에 학습 성능이 크게 향상된다.
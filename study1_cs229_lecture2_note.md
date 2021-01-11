# Machine Learning
: find a model and its parameter so that the resulting predictor performs well.

Training Data -> model (theta) -> Test Data

Training Data : {(x1, y1), (x2, y2) ... (xn, yn)}
Test Data : {(x1', y1'), (x2', y2') ... (xn', yn')}

P(y' | x', D)
> x' 예측하고싶은 집의 특성   
> D  집값 데이터   
> y' 예측한 집값   

앙상블하면 distribution을 모델링하기에 더 좋다

입학사정관
출력값이 합격 불합격 뿐 아니라 distribution 및 sigma를 함께 주어야..


최성준 교수님
bayesian neural net
https://www.edwith.org/bayesiandeeplearning/lecture/24678/

hessian matrix를 (2계도 함수로) 계산하는 건 너무 computation이 커서 잘 안씀.. 그래서 newtons method를 잘 안씀

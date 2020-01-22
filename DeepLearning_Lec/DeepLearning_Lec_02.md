### DEEPLEARNING LEC 02 : Linear Regression의 가정과 cost function

<br/>

#### Linear Regression

<img src="https://user-images.githubusercontent.com/45492242/72896424-16b15b00-3d63-11ea-8e48-d7f5d16905c4.JPG" alt="IMG_0988" style="zoom: 50%;" />

좌측 : Data / 우측 : Presentation

<br/>

#### Linear Hypothesis

Linear Model이 우리의 Data에 잘 맞을 것이라는 가정을 세움

*실세계에서 linear model이 적용 가능한 경우가 많음*

**학습** : Data에 잘 부합하는 Linear Equation 찾는 과정

<img src="https://user-images.githubusercontent.com/45492242/72896653-99d2b100-3d63-11ea-98dc-3c1d5e56feec.jpeg" alt="IMG_DF73B1751B8C-1" style="zoom:67%;" />



좌측의 각 선은 H(x) = Wx + b 로 표현된다.

선들 중 어느 선이 Data에 가장 잘 맞는지 판단할 수 있어야한다.

즉, 최선의 W(weight)와 b(bias)의 값을 찾아내야한다.

<br/>

<img src="https://user-images.githubusercontent.com/45492242/72897374-2c278480-3d65-11ea-84b0-a6f8f7c7bc18.JPG" alt="IMG_D33C3AA4E44D-1" style="zoom:67%;" />

실제 data와 hypothesis 간의 거리를 측정하여 최선의 hypothesis (이전 그림의 line들 중에서) 를 찾아낸다.

<br/>

#### Cost Function (= Loss Function)

How fit the line to our training data를 측정하는 함수

<br/>

$H(x)-y$ : 가장 단순한 방식. 부호가 발생한다는 단점이 있다.

$(H(x)-y)^2$ : 가장 기본적인 방식. 부호가 없어서 편리하다. 

​					  	 차이가 작을 때 보다 차이가 클 때 더 많은 penalty를 부여할 수 있다.

<br/>

$cost(W,b) = 1/m \sum_{i=1}^m (H(x_i)-y)^2  $  *(m : training data set의 data 개수)*

<br/>

**Linear Regression 의 학습 목표 : ** $cost(W,b)$ 를 최소화 시키는 W, b의 값 찾는 것!
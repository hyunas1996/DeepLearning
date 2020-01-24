#### DEEPLEARNING LAB 01 : 개발 환경 구성

##### 아나콘다 설치하기

[아나콘다 공식 다운로드 페이지](https://www.anaconda.com/ ) 에서 python 3.7 version을 설치한다. <br/>

터미널에서 `$ conda list ` 를 입력하면 출력되는 리스트들 중에서 필요한 것을 골라 설치할 수 있다. <br/>

*zsh: command not found: conda* 메세지가 출력될 경우, <br/>

`vim ~/.zshrc` 마지막에 `export PATH="/Users/사용자이름/anaconda/bin:$PATH"`  을 추가한다.<br/>

<br/>

##### 환경 구성

###### 1) 아나콘다 가상환경 만들기

`Python-V` 를 이용해서 python의 버전을 확인한다. (my case : 3.6.0)<br/>

아나콘다 가상환경 생성 : `conda create -n wikiml python=3.6.0` 을 입력한다. <br/>

아나콘다 wikiml 가상환경 활성화 : `source activate wikiml`<br/>

<br/>

wikiml 은 DeepLearning Lab 시리즈의 실습 프로젝트를 실행할 가상환경이다.<br/>

이제부터는 wikiml에 파이썬 데이터 패키지를 수동으로 설치 해 보겠다.<br/>

자동으로 설치하는 방식이 있지만, 머신러닝 관련 파이썬 라이브러리에 익숙 해 지기 위해서 수동 설치를 택한다.<br/>

<br/>

###### 2)  Pandas

pandas는 데이터를 수정하고 변경하는 데 사용되는 파이썬 라이브러리로, data analysis에 사용되는 대표적인 라이브러리다.<br/>

pands 설치 : `pip install pandas` <br/>

<br/>

###### 3) NumPy

numpy는 머신러닝의 입력값으로 사용되는 vector, matrix 등을 수정하고 변경하는 데 사용되는 파이썬 라이브러리다.<br/>

고성능 수치 계산을 위해서 만들어 졌으며, 메모리를 효율적으로 사용할 수 있다.<br/>

numpy 설치 : `conda install numpy`<br/>

<br/>

###### 4) Keras

Keras는 딥러닝 모델을 손쉽게 구현하고 실험하기 위한 딥러닝 상위 레벨의 인터페이스를 제공하는 파이썬 라이브러리다. <br/>

Keras 설치 : `pip install keras`<br/>

<br/>

###### 5) TensorFlow

텐서플로우는 구글에서 제공하는 딥러닝 모델의 상용화에 중접을 둔 파이썬 라이브러리다. <br/>

텐서플로우 자체는 C++로 구현되어 있으나, python, java 등 다양한 언어를 지원한다. <br/>

TensorFlow 설치 : `pip install tensorflow`

<br/>

###### 6) scikit-learn 

통상적으로 머신 러닝은 텐서플로우를 많이 사용한다. 상대적으로 텐서플로우는 low-level 라이브러리에 가깝고 scikit-learn (사이킷-런) 은 high-level 라이브러리에 가깝다. <br/>

텐서플로우는 딥러닝에 사이킷-런은 데이터 마이닝과 머신러닝에 적용하기 적합하다. <br/>

scikit-learn 설치 : `conda install scikit-learn`

<br/>

###### 7) seaborn

seaborn은 Matplotlib을 기반으로 다양한 색상 테마와 통계용 차트 기능을 추가한, 데이터 시각화를 위한 파이썬 라이브러리이다. <br/>

seaborn 설치 : `conda install seaborn`

<br/>

###### 8) Jupyter notebook 

jupyter notebook은 브라우저에서 작동하는 파이썬 코드 작성 도구이다. 가독성을 높여주며 데이터를 시각화 할 때 편리하다. <br/>

jupyter notebook 설치 : `conda install jupyter notebook`

<br/>
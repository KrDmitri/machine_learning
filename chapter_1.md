## 인공지능이란?
인공지능(artificial intelligence)은 사람처럼 학습하고 추론할 수 있는 지능을 가진 컴퓨터 시스템을 만드는 기술입니다.  

## 머신러닝이란?
머신러닝 machine learning은 규칙을 일일이 프로그래밍하지 않아도 자동으로 데이터에서 규칙을 학습하는 알고리즘을 연구하는 분야  

## 딥러닝이란?
많은 머신러닝 알고리즘 중에 인공 신경망(artificial neural network)을 기반으로 한 방법들을 통칭하여 딥러닝(deeplearning)이라고부릅니다. 종종사람들은 인공신경망과딥러닝을크게 구분하지 않고사용합니다.  

## 머신러닝 라이브러리
사이킷런, 텐서플로, 파이토치(텐서플로와 파이토치는 딥러닝에 쓰임)

## 파이썬에서 과학계산용 그래프 그리기 matplotlib
Import matplotlib.pyplot as plt  

## list 두 개 더하기
```python
length = bream_length + smelt_length
```
위 코드는 도미 길이 데이터와 빙어 길이 데이터를 한 컬럼에 모아준다.  

## zip() 함수
zip() 함수는 나 열된 리스토에서 원소를 하나씩 꺼내주는 일을 합니다.  

## KNeighborsClassifier
```python
from sklearn.neighbors import KNeighborsClassifier ##필요한 함수 임포트
kn = KNeighborsClassifier()                        ##모델 객체 생성
kn.fit(fish_data, fish_target)                     ##모델 학습
kn.score(fish_data, fish_target)                   ##모델 성능 검사
```

## K-최근접 이웃 알고리즘
k一최근접 이웃 알고리 즘은 매우 간단합니다. 어떤 데이터에 대한 답을 구할 때 주위의 다른 데이터를 보고 다수를 차지하는 것을 정답으로 사용합니다.  
이렇게 생각하면 k―최근접 이웃 알고리즘을 위해 준비해야 할 일은 데이터를 모두 가지고 있는 게 전부입니다. 새로운 데이터에 대해 예측할 때는 가장 가까운 직선거리에 어떤 데이터가 였는지를 살 피기만 하면 됩니다. 단점은 k―최근접 이웃 알고리즘의 이런 특징 때문에 데이터가 아주 많은 경우 사용하기 어렵습니다. 데이터가 크기 때문에 메모리가 많이 필요하고 직선거리를 계산하는 데도 많 은시간이 필요합니다.  

## 변수 n_neighbors
K-최근접 이웃 알고리즘은 가까운 몇개의 변수를 참고할까? KNeighborsClassifier 클래 스의 기본값은 5입니다. 이 기준은 n_neighbors 매개변수로 바꿀 수 있습니다.  
예시 :  
```python 
KNeighborsClassifier(n_neighbors=49) # 참고데이터를49개로한kn49 모델
```
위 코드는 너무 많은 주변 데이터를 참고하기 때문에 정확도가 떨어짐  

## KNeighborsClassifier 클래스의 fit(), score(), predict() 메서드
fit() : 모델을 학습하는 코드로 특성과 정답 데이터를 전달한다.  
score() : 모델의 성능을 확인하는 코드  
predict() : 테스트 데이터가 있으면 그 데이터의 타겟 데이터를 알 수 있다.  

## 전체 소스 코드
https://colab.research.google.com/drive/1V3tY0RsfCjHgDoSN2VadTJjIbrd8V-nE#scrollTo=lrkcnZ8Q4CoR

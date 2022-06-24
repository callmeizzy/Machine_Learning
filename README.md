# Machine Learning

## <chapter 1>

♣ 머신러닝 차원축소 ♣

변수(피쳐 혹은 컬럼이라고도 함) 의 조합을 통해 새로운 변수 발견

### 1. Feature Selection

가지고 있는 변수들 중에 의미있는 변수만 선택

변수를 선택하는 방법은 주로 상관분석을 이용(공분산과 상관계수)

### 2. Feature Extraction
변수추출 (1,2,3 번 변수를 조합해서 A,B라는 새로운 변수를 생성)

주로 사용되는 방법은 주성분분석(PCA : Principal Componene Analysis)

PCA 실행결과 나온 Variance를 그래프로 그린 뒤 급격하게 떨어지는 지점에서 PC개수 선택

#### 2.1 PCA?

분산이 최대인 축 찾기

찾은 축과 직교하면서 분산이 최대인 두번째 축 찾기

첫번째 축과 두번째 축에 직교히고 분산을 보존하는 세번째 축 찾기

#### 2.2 정규화

PCA를 위해서 반드시 필요함

스케일이 다르면 분산이 다름




## <chapter 2>
♣군집화 (클러스터링)♣

비슷한 성향을 가진 그룹을 찾을 수 있음
우리는 그 중 군집화의 알고리즘 K-Means를 사용하겠다

### K-Means 특징
전체 data를 k개로 군집화 하겠다는 뜻

거리를 이용한 분류 / 연속형 범주에 적합한 모델

반복된 작업을 수행 (euclidian 거리기법)

짧은 계산 시간

주어진 자료에 대한 사전정보 없이 의미있는 자료구조 찾기 가능

범주형(카테고리형) 변수를 다룰 경우 주의


### K-Means 순서
#### 1. KMeans(n_cluster = k)

주어진 값들 사이의 거리 혹은 유사성을 이용하여 분류

전체 데이터를 k개의 집단으로 그룹화

데이터를 기준점 중심으로 euclidian 거리가 최소가 되도록 k개의 그룹으로 군집

군집 별 중심 값에서 중심과의 거리를 기반으로 데이터를 분류하는 군집기법

#### 2. Kmeans.fit()
학습시키기

#### 3. KMeans.inertia_

학습된 KMeans의 응집도를 확인

응집도란 각 데이터로부터 자신이 속한 군집의 중심까지의 거리를 의미

즉, 낮을수록 군집화가 더 잘 되어있다

#### 4. KMeans.predict(data)
학습된 데이터를 바탕으로 데이터를 변환시켜줌




3. KNN

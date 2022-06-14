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

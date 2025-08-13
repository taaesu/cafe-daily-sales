# Maven Roasters 일별 매출 분석 및 예측



\## 프로젝트 개요

뉴욕에 위치한 가상의 커피 전문점 "Maven Roasters"의 거래 데이터를 활용하여

일별 매출액의 변화 추세를 분석하고, 향후 매출을 예측하는 모델을 구축하였습니다.



\## 데이터셋

\- 파일명 : Coffee\_Shop\_Sales.xlsx



\## 데이터 전처리

\- 결측치 없음

\- 일별 매출 집계

\- 필요 없는 컬럼 제거



\## 분석 내용

1\. EDA

   - 일별 매출 분포 확인

   - 제품 카테고리별 매출 분석 → 커피 카테고리 매출 비중이 가장 큼

   - 매장별/요일별 매출 차이 분석 → 유의미한 차이 없음

   - 시간 경과에 따른 매출 증가 추세 확인



2\. 모델링

   - 적용 모델: 선형회귀, Ridge, Lasso, RandomForest, XGBoost, SARIMA, SARIMAX

   - 평가 지표: RMSE (학습:검증 데이터 분할)

   - XGBoost 모델이 가장 우수 (RMSE 60 → 튜닝 후 57)



3\. 변수 중요도

   - XGBoost 모델 기준으로 'unit\_price'와 'transaction\_qty'가 매출 예측에 가장 큰 영향을 줌



\## 사용 기술

\- Python (pandas, numpy, matplotlib, seaborn, scikit-learn, xgboost, statsmodels, scipy)

\- Jupyter Notebook


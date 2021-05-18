# LSTM 신경망을 사용한 시계열 데이터 예측
* data : 15분 간격의 시계열 데이터
* input :  온도, 습도, 요일, 사용량(이전) 
* output : 사용량(192 step 후)

### 데이터 전처리
* 비정상 데이터 제거
* datetime 요일 추가 
* 전처리 전
![before_cleaning](https://user-images.githubusercontent.com/84064361/118604783-849f5280-b7f0-11eb-834a-95e274a0a924.png)

* 전처리 후
![after_cleaning](https://user-images.githubusercontent.com/84064361/118604787-86691600-b7f0-11eb-9ce1-edf92a2d251c.png)

### 학습-예측
* 학습 데이터
![traindata](https://user-images.githubusercontent.com/84064361/118593837-52d3bf00-b7e3-11eb-8163-e4b6fad7a8bd.png)ㅑ

* 예측 결과
![testdata](https://user-images.githubusercontent.com/84064361/118593842-55361900-b7e3-11eb-90ad-f7f2b36d5eb5.png)


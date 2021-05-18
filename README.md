# LSTM 신경망을 사용한 시계열 데이터 예측
* data : 15분 간격의 시계열 데이터
* input :  온도, 습도, 요일, 사용량(이전) 
* output : 사용량(192 step 후)

### 데이터 전처리
* 비정상 데이터 제거
* 전처리 전
![before_cleaning](https://user-images.githubusercontent.com/84064361/118604783-849f5280-b7f0-11eb-834a-95e274a0a924.png)

* 전처리 후
![after_cleaning](https://user-images.githubusercontent.com/84064361/118604787-86691600-b7f0-11eb-9ce1-edf92a2d251c.png)

* datetime에 해당 요일 추가
![head](https://user-images.githubusercontent.com/84064361/118623039-d0f38e00-b802-11eb-88a4-4979c8e5ea50.png)

### 학습-예측
* 2개의 LSTM layer와 한개의 Dense layer로 이루어진 네트워크로 시퀀스 학습
![model_plot](https://user-images.githubusercontent.com/84064361/118617182-596f3000-b7fd-11eb-8e98-b42115514782.png)

* 과거의 패턴을 학습하여 미래 사용량을 예측

* 학습 데이터 (사용량) 패턴(20,130 행)
![traindata](https://user-images.githubusercontent.com/84064361/118593837-52d3bf00-b7e3-11eb-8163-e4b6fad7a8bd.png)

* 테스트 데이터(사용량) 예측 결과(5,033 행)
![testdata](https://user-images.githubusercontent.com/84064361/118593842-55361900-b7e3-11eb-90ad-f7f2b36d5eb5.png)


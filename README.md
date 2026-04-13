# **Datasets**
- UCI HAR (Human Activity Recognition)
- 무엇을 측정한 데이터인가?
  - 사람이 스마트폰을 허리에 착용하고 6가지 동작을 수행했을 때, 폰 안에 들어있는 두 가지 핵심 센서의 값을 기록한 데이터
  - Accelerometer : 가속도 센서 (움직임의 세기, 중력의 방향, 급격한 속도 변화 등)
  - Gyroscope : 자이로스코프 센서 (스마트폰이 얼마나 회전하는지, 어떤 각도로 기울어져 있는지)
- 맞혀야 할 정답(Label)은?
  - 이 사람이 지금 무엇을 하고 있는지
    1. Walking (걷기)
    2. Walking Upstairs (계단 오르기)
    3. Walking Downstairs (계단 내려가기)
    4. Sitting (앉아 있기)
    5. Standing (서 있기)
    6. Laying (누워 있기)
- X / y 데이터 형태
  - 초당 수십 번씩 파동하는 복잡한 센서 신호 > 분석하기 좋게 미리 *561개의 특징(Features)*으로 가공해둔 상태
  - ex. avg, max, min ... > 숫자들이 한 세트가 되어서 > 이 신호는 '걷기'이다.


 
# **Model**
- CNN
- RNN
- LSTM

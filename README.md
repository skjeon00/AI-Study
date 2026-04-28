# **Wild-SHARD (Smartphone-based HAR Dataset)**
- Data Definition : 무엇을 측정한 데이터인가?
  - 출처 및 수집자
    - 일상적인 환경(In-the-wild)에서 스마트폰을 사용하는 불특정 다수의 사용자들로부터 수집된 데이터
  - 측정 내용
    - 스마트폰에 내장된 6가지 센서(가속도계, 자이로스코프) 및 기타 파생 센서(중력, 회전 등)를 통해
    - 사용자의 움직임을 시계열 데이터로 기록
  - 특징
    - 사용자가 폰을 쥐는 방향, 주머니 위치, 걷는 습관 등이 모두 제각각인 '실제 상황(Real-world context)' 데이터
- Project Goal : 맞춰야 할 정답(Label)은?
  - 목표: 딥러닝 모델(CNN 등)을 사용하여 복잡한 센서 신호로부터 사람의 6가지 주요 행동을 자동으로 분류
  - Label: Downstairs, Running, Sitting, Standing, Upstairs, Walking
- Feature Selection : 사용할 주요 데이터 요소
  - X: '가속도'와 '자이로' 센서 값 + 'Magnitude' (Feature Engineering)
  - y: 'activity'
<br>
<br>

# **UCI HAR 데이터셋과의 차이점**
| 비교항목 | UCI | Wild |
| :---: | :---: | :---: |
| **비교 항목** | **UCI HAR** | **Wild-SHARD** |
| **수집 환경** | 통제된 실험실 (특정 위치에 기기 고정) | 실제 일상 (사용자별 기기 위치 상이) |
| **데이터 품질** | 노이즈↓, 규칙적인 패턴 | 현실적인 노이즈, 불규칙한 패턴 |
| **일반화 성능** | 실험실 환경 외 정확도가 떨어질 수 있음 | 실제 앱에 적용 시 더 높은 정확도 유지 가능 |
| **분석 난이도** | 상대적으로 낮음 (교과서적 데이터) | 높음 (전처리와 피처 엔지니어링의 역할이 큼) |
<br>
<br>

# **Model**
- CNN
<br>
<br>

# tabular_data

## EDA 체크리스트

### 1. 데이터 로드

- 데이터 섞기(랜덤 섬플링)
- 메모리 사용량 줄이기

### 2. 데이터 확인

- 훈련, 테스트 데이터의 칼럼이 같은지 확인
- 변수의 자료형 확인
- 중복 row & 중복 column 확인, 제거

- 메타 데이터 생성
- 분석노트 엑셀파일 생성

- Null 체크

- Target 분포 확인
  - Classification
    - binary classification 문제의 경우 1과 0의 분포에 따라 모델 평가 방법이 달라진다.
    - costa rican처럼 세대주의 target만 카운트해야 하는 경우도 있다
    - target label이 불균형 할 때
      - under sampling
      - over sampling

  - Regression
    - Target 값이 양수인 경우 (거리, 길이 등), 로그 정규분포일 수도 있다. => 로그 변환 필요 => 마지막에 예측값을 np.exp()를 적용해야 한다
    - (log1p(x) == log(x + 1))을 원래대로 되돌리려면?



## Preprocessing 체크리스트

### 1. 데이터 merge

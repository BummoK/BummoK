# 정상 동작 학습을 활용한 낙상 이상치 검출 연구

[포트폴리오](../README.md) · [English overview](../README.en.md)

> **English summary:** Investigated anomaly detection for falls from January to August 2023. Explored GANomaly and autoencoder-based approaches trained on normal motions, then examined the limitations of reconstruction-based detection before impact and investigated time-series prediction.

**핵심 기여** · 사전에 수집하지 못한 낙상 동작에 대응하기 위해 문제를 다시 정의하고, 충격 전 검출에서 드러난 한계를 분석했습니다.

## 1. 프로젝트와 역할

- **기간:** 2023.01–2023.08.
- **담당:** 이상치 검출 모델 구현, IMU 시계열 적용 및 결과 분석.
- **기술:** Python, TensorFlow, GANomaly, Autoencoder, ConvLSTM.

## 2. 문제 정의

낙상·일상동작의 이진 분류는 학습 데이터에 없는 낙상에 어떻게 대응할 것인지가 과제였습니다. 정상 동작만으로 모델을 학습하고 정상 패턴에서 벗어나는 움직임을 탐지하는 접근을 검토했습니다.

## 3. 연구 과정

1. GANomaly와 Autoencoder 계열 모델을 구현하고 KFall·FARSEEING 데이터를 활용했습니다.
2. ConvLSTM과 Autoencoder를 결합해 신호를 재구성하는 방식도 검토했습니다.
3. 충격 후 검출과 충격 전 검출의 결과가 다르다는 점에 주목했습니다. 충격 전에는 큰 충격 신호를 사용할 수 없어 정상·이상 동작을 구분하기 어려웠습니다.
4. 과거 신호로 이후 시계열을 예측하고 이를 이상치 검출에 활용하는 방향을 탐색했습니다.

## 4. 결과와 해석

- 미관측 동작 대응을 목표로 정상 동작 학습이라는 대안을 검토했습니다.
- 한 접근의 성능이 낮게 나타났을 때 검출 시점과 사용 가능한 신호를 기준으로 원인을 분석했습니다.
- 기존 포트폴리오에는 예측 방식의 후속 탐색과 논문 준비 단계까지 기록되어 있습니다. 게재가 확인된 논문이나 상용 검증 완료 모델로 제시하지 않습니다.

원본 실행 로그와 데이터 분할을 재확인하지 않은 과거 도표의 정확도·임계값은 재사용하지 않았습니다. 현재 제품의 최종 판정 알고리즘과도 구분합니다.

---

[현재 프로젝트의 오류 분석](02-evaluation.md) · [전체 포트폴리오](../README.md)

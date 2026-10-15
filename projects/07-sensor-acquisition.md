# 알고리즘 연구를 위한 센서·영상 수집 환경

[포트폴리오](../README.md) · [English overview](../README.en.md)

> **English summary:** Developed instrumentation and GUI workflows during graduate research, including IMU acquisition and synchronized sensor/video storage in LabVIEW. Connected experimental data collection with feature extraction and ANN-based post-fall detection research.

**핵심 기여** · 모델 학습 이전의 센서 계측·실험 데이터 수집·분석 도구를 함께 개발했습니다.

## 1. 문제와 역할

낙상 검출 모델을 평가하려면 센서 신호가 어떤 동작에서 발생했는지 확인할 수 있어야 합니다. 센서 데이터와 영상이 따로 저장되면 동작의 시작과 충격 시점을 대조하기 어려워, 신호와 영상을 함께 확인할 수 있는 수집 환경을 구성했습니다.

## 2. 구현과 연구 흐름

1. **센서 수집:** 연구실 선배와 협업해 MPU9250 IMU와 nRF52832 모듈을 이용한 수집 환경을 구성하고 IAR 기반 펌웨어 적용과 RF 통신을 다뤘습니다.
2. **GUI 개발:** LabVIEW로 웹캠 영상과 IMU 신호를 동기화해 저장하는 도구를 개발했습니다.
3. **실험·분석:** 낙상·일상동작 데이터를 수집하고 특성벡터를 추출했습니다.
4. **모델 비교:** 랭킹 알고리즘에 따른 특성 조합과 ANN 모델을 연구했습니다.

추가 연구 업무에서는 PyQt·.NET 기반 센서 데이터 활용 GUI도 다뤘습니다. 회로·펌웨어 전부의 단독 설계로 표현하지 않고, 직접 개발한 GUI와 협업한 수집 환경을 구분합니다.

## 3. 연구로 이어진 결과

- *Post-fall Detection Using ANN Based on Ranking Algorithms* — **제1저자**, *International Journal of Precision Engineering and Manufacturing*, 21, 1985–1995 (2020).
- *The Performance of Post-Fall Detection Using the Cross-Dataset: Feature Vectors, Classifiers and Processing Conditions* — **제1저자**, *Sensors*, 21(14), 4638 (2021). [논문](https://doi.org/10.3390/s21144638)

센서 수집과 특성 기반 연구는 이후 딥러닝·모바일 개발의 기반이 됐습니다. 충격 후 낙상 검출 연구의 결과를 현재 충격 전 검출 알고리즘의 성능으로 대체하지 않습니다.

---

[연구 배경](../research.md) · [모바일 센서 앱](04-android-sensor-app.md)

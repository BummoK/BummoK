# TinyFallNet: 충격 전 낙상 검출 모델 경량화

[포트폴리오](../README.md) · [English overview](../README.en.md)

> **English summary:** First author of TinyFallNet, published in *Sensors* in 2023. Benchmarked ConvLSTM, investigated VGG/ResNet architectures and simplified the model for IMU-based pre-impact fall detection, including evaluation on recorded older-adult data.

**핵심 기여** · 웨어러블 환경의 제약을 고려해 모델 구조를 분석하고, 경량화와 데이터 조건별 평가를 연결했습니다.

## 1. 프로젝트와 역할

- **연구 기간:** 2022.01–2022.12로 정리된 경량화 프로젝트. 논문은 2023년 게재.
- **기술:** Python, TensorFlow, ConvLSTM, VGGNet, ResNet.
- **역할:** 제1저자. 논문 기여 명세에 연구 구상, 방법론, 소프트웨어, 검증·분석, 초고 작성과 시각화가 기재되어 있습니다. [논문과 기여 명세](https://pmc.ncbi.nlm.nih.gov/articles/PMC10610937/)

## 2. 해결해야 했던 문제

충격 전에 낙상을 판단하는 모델은 검출 성능뿐 아니라 착용형 장치에서 실행할 수 있는 크기와 구조를 함께 고려해야 합니다. 학습에 사용한 젊은 성인의 동작에서 좋은 결과를 얻더라도 고령자 동작에 그대로 적용되는지는 별도 확인이 필요했습니다.

## 3. 연구 접근

1. 선행 ConvLSTM 모델을 벤치마킹하고 VGGNet·ResNet의 구조를 비교했습니다.
2. IMU 시계열에 맞춰 구조를 단순화하며 TinyFallNet을 제안했습니다.
3. KFall 기반 모델 개발과, FARSEEING 낙상·KFall 고령자 일상동작에 대한 저장 데이터 평가를 나눴습니다.
4. 고령자 동작에서 나타난 오탐을 분석하고 시계열 판정 방식을 검토했습니다.

## 4. 결과와 적용 범위

- **제1저자 논문:** Koo, B., et al. (2023). *TinyFallNet: A Lightweight Pre-Impact Fall Detection Model*. **Sensors, 23(20), 8459**. [DOI](https://doi.org/10.3390/s23208459)
- 모델 구조의 경량화와 고령자 데이터에 대한 평가를 논문으로 정리했습니다.
- 후속 모바일 개발에서는 모델을 Android 실행 환경에 통합했습니다. [앱 개발 사례](04-android-sensor-app.md)

논문의 저장 데이터 평가는 현재 회사의 알고리즘 1.3.5 재생 비교와 별개의 연구입니다. MCU 임베딩을 목표로 한 경량화 연구와 특정 MCU에서의 최종 제품 검증도 구분합니다. 이 페이지에서는 연구 간 성능 수치를 직접 비교하지 않습니다.

---

[연구·논문 목록](../research.md) · [현재 프로젝트의 배포 검증](03-deployment-verification.md)

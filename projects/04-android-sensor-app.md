# BLE 센서와 AI 추론을 연결한 Android 앱

[포트폴리오](../README.md) · [English overview](../README.en.md)

> **English summary:** Developed a research Android app from September 2023 to January 2024 using Kotlin and Jetpack Compose. Integrated BLE sensor connectivity, IMU charts, data storage and TensorFlow Lite inference to display movement-related model outputs.

**핵심 기여** · 연구용 모델을 센서 연결·데이터 확인·추론 결과 표시가 가능한 모바일 소프트웨어로 연결했습니다.

## 1. 프로젝트와 역할

- **기간:** 2023.09–2024.01.
- **환경:** 연세대학교 생체역학연구실의 박사후연구원 업무.
- **담당:** Android 애플리케이션 개발과 딥러닝 모델 통합.
- **기술:** Android Studio, Kotlin, Jetpack Compose, BLE, TensorFlow Lite, Git.

## 2. 해결해야 했던 문제

IMU 기반 낙상 검출·동작 인식·위험도 예측 알고리즘을 확인하려면 센서 신호와 모델의 출력을 같은 흐름에서 볼 수 있어야 했습니다. 센서 통신과 모델 실행이 분리된 상태에서는 입력이 정상적으로 들어오는지, 어떤 움직임에 모델이 반응하는지 확인하기 어려웠습니다.

## 3. 구현한 흐름

1. **센서 연결:** BLE 스캔과 연결 기능을 구현하고 Arduino Nano 33 BLE Sense의 IMU 데이터를 수신했습니다.
2. **신호 확인:** 가속도·각속도 데이터를 차트로 표시하고 측정 데이터를 저장하는 기능을 구성했습니다.
3. **모델 실행:** TensorFlow 모델을 TensorFlow Lite로 변환해 모바일 앱에 통합했습니다.
4. **결과 표시:** 낙상 여부와 수행 동작 등 모델 출력을 화면에 표시했습니다.

`IMU 센서 → BLE 수신 → 신호 차트·저장 → TFLite 추론 → 결과 표시`

## 4. 결과와 배운 점

- 기존 포트폴리오에는 BLE 연결, 센서 데이터 출력·저장, 딥러닝 결과 표시 화면이 남아 있습니다.
- 모델 개발 경험을 바탕으로 센서 입력과 추론 결과를 연결하는 연구용 앱을 개발했습니다.
- 모델 크기와 실행 환경을 함께 검토하며 MCU와 모바일의 적용 조건이 다름을 다뤘습니다.

이 사례는 당시 연구용 앱 개발 경험입니다. 앱스토어 출시, 사용자 규모, 처리 지연이나 배터리 성능을 측정한 사례로 제시하지 않습니다. 현재 회사 프로젝트의 앱 전체를 단독 개발했다는 의미도 아닙니다.

---

[모델 경량화 연구](05-tinyfallnet.md) · [전체 포트폴리오](../README.md)

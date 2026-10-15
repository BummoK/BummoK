<p align="center"><img src="https://raw.githubusercontent.com/BummoK/BummoK/main/assets/cover.svg" alt="Biomedical AI — Sensor algorithms, evaluation and software" width="100%"></p>

<p align="center"><strong>의공학 박사 · AI 알고리즘 및 소프트웨어 개발 약 3년</strong><br>센서 데이터에서 알고리즘 개발, 성능 평가와 개선까지</p>

<p align="center"><a href="https://github.com/BummoK/BummoK/blob/main/README.en.md">English</a> · <a href="https://github.com/BummoK/BummoK/blob/main/projects/01-sensor-ai.md">AI 개발</a> · <a href="https://github.com/BummoK/BummoK/blob/main/projects/02-evaluation.md">평가와 개선</a> · <a href="https://github.com/BummoK/BummoK/blob/main/projects/03-deployment-verification.md">배포 검증</a></p>

## 안녕하세요

**사람의 움직임을 분석하는 AI 알고리즘을 개발합니다.** 의공학 연구 배경을 바탕으로 웨어러블 낙상 감지 프로젝트의 알고리즘 개발·성능 평가·개선 전반을 담당했습니다.

```python
background = "Biomedical Engineering, PhD"
focus = ["Sensor AI", "Wearable Healthcare"]
work = ["Develop", "Evaluate", "Improve"]
```


## 만들고 개선한 것들

### 웨어러블 IMU 기반 낙상 감지

낙상과 일상동작을 구분하면서 오경보와 검출 시점을 함께 고려하는 알고리즘 개발. **하나의 프로젝트를 세 가지 업무 관점**으로 정리했습니다.

<a href="https://github.com/BummoK/BummoK/blob/main/projects/01-sensor-ai.md"><img src="https://raw.githubusercontent.com/BummoK/BummoK/main/assets/case-01.svg" alt="01 Sensor AI — IMU preprocessing, model development and adaptation" width="100%"></a>

낙상과 유사한 일상동작을 다루기 위해 센서 전처리, 모델 학습·전이학습과 **AI 추정과 물리적·시계열적 움직임 특성을 종합한 판정**을 연결했습니다.

[개발 접근과 담당 업무 →](https://github.com/BummoK/BummoK/blob/main/projects/01-sensor-ai.md)

<a href="https://github.com/BummoK/BummoK/blob/main/projects/02-evaluation.md"><img src="https://raw.githubusercontent.com/BummoK/BummoK/main/assets/case-02.svg" alt="02 Evaluation — Trial-level errors, timing and replay input investigation" width="100%"></a>

동작 시행별 오탐·미탐과 검출 시점을 분석했습니다. 미검출로 표시된 사례에서 오래된 모델 출력이 재생 입력에 사용된 경로를 추적한 조사 과정을 소개합니다.

[평가 설계와 원인 분석 →](https://github.com/BummoK/BummoK/blob/main/projects/02-evaluation.md)

<a href="https://github.com/BummoK/BummoK/blob/main/projects/03-deployment-verification.md"><img src="https://raw.githubusercontent.com/BummoK/BummoK/main/assets/case-03.svg" alt="03 Verification — Model artifacts, native execution and recorded-data replay" width="100%"></a>

배포 모델과 실행 경로를 구분해 동작을 비교했습니다. **5,912개 저장 시행**의 호스트 재생 조사에서 판정 일치와 첫 검출 시점의 차이를 각각 확인한 사례입니다.

[비교 조건과 검증 결과 →](https://github.com/BummoK/BummoK/blob/main/projects/03-deployment-verification.md)

## 이렇게 일합니다

<img src="https://raw.githubusercontent.com/BummoK/BummoK/main/assets/workflow.svg" alt="IMU signals → model development → trial evaluation → integration checks, with an improvement loop" width="100%">

1. **평가 단위부터 정합니다.** 학습 창의 분류 정확도와 원본 시행의 검출 결과를 구분합니다.
2. **실패를 시간축에서 분석합니다.** 센서 신호, 모델 출력과 첫 검출 시점을 함께 확인합니다.
3. **개선의 영향을 함께 봅니다.** 오탐 감소, 검출 지연과 기존 동작의 회귀를 비교합니다.
4. **결과를 다시 추적할 수 있게 합니다.** 입력, 모델, 판정 버전과 실행 경로를 연결합니다.

## 사용하는 도구

<p><img src="https://raw.githubusercontent.com/BummoK/BummoK/main/assets/badge-python.svg" alt="Python" height="30"> <img src="https://raw.githubusercontent.com/BummoK/BummoK/main/assets/badge-tensorflow.svg" alt="TensorFlow" height="30"> <img src="https://raw.githubusercontent.com/BummoK/BummoK/main/assets/badge-tflite.svg" alt="TensorFlow Lite" height="30"> <img src="https://raw.githubusercontent.com/BummoK/BummoK/main/assets/badge-numpy.svg" alt="NumPy" height="30"> <img src="https://raw.githubusercontent.com/BummoK/BummoK/main/assets/badge-pandas.svg" alt="pandas" height="30"></p>

| 영역 | 프로젝트에서 사용한 기술 |
|:---|:---|
| 모델 개발 | Python · TensorFlow · Keras · TensorFlow Lite |
| 센서 데이터와 평가 | NumPy · pandas · SciPy · IMU 시계열 · 시행 단위 오류 분석 |
| 알고리즘 적용 검증 | C/C++ 네이티브 실행 비교 · DLL 재생 평가 · ARM 대상 알고리즘 통합 |

## 관심 분야와 연락처

Deep Learning · TinyML · 웨어러블 헬스케어

이메일: [koobummo726@gmail.com](mailto:koobummo726@gmail.com)

<sub>사례의 수치는 저장 데이터의 개발·회귀 검증 기록입니다. 실제 기기의 최종 알람 및 현장 성능과 구분하며, 평가 조건은 각 사례에 기재했습니다.</sub>

<p align="center"><img src="https://raw.githubusercontent.com/BummoK/BummoK/main/assets/cover.png" alt="안경 쓴 구범모 아바타와 Sensor AI 포트폴리오 배너" width="100%"></p>

<p align="center"><strong>구범모 · Bummo Koo</strong><br>의공학 박사 · 세이프웨어 알고리즘 개발팀 팀장 / 책임연구원</p>

<p align="center"><a href="https://github.com/BummoK/BummoK/blob/main/README.en.md">English</a> · <a href="https://github.com/BummoK/BummoK/blob/main/research.md">연구·논문</a> · <a href="https://github.com/BummoK/BummoK/blob/main/funded-projects.md">정부·기업 과제</a> · <a href="mailto:koobummo726@gmail.com">Email</a></p>

## 안녕하세요 👋

**센서로 사람의 움직임을 읽고, 이를 AI 알고리즘과 소프트웨어로 만드는 구범모입니다.** 연세대학교에서 의공학 박사학위를 받았고, 2024년 5월부터 세이프웨어에서 웨어러블 낙상 감지 알고리즘을 개발하고 있습니다.

낙상을 얼마나 잘 찾는지뿐 아니라 **얼마나 일찍 알아채는지, 일상생활에서 불필요한 경보를 줄일 수 있는지**에 관심이 많습니다. 실험 데이터를 직접 모으는 일부터 모델 개발·평가, 센서 관리 앱과 분석 도구를 만드는 일까지 해 왔습니다.

## 🔬 연구 · 움직임을 이해하고 위험을 알아채기

### TinyFallNet — 충격 전 낙상 검출 모델 경량화

웨어러블 장치에 적용하기 위해 ResNet 구조를 줄이고, 고령자 데이터에서 오경보와 검출 시점을 분석했습니다. **2023년 Sensors 제1저자 논문**으로 발표했습니다.

![TinyFallNet 모델 구조](https://raw.githubusercontent.com/BummoK/BummoK/main/assets/research/tinyfallnet-architecture.png)

*Koo et al., 2023, Figure 4. [논문](https://doi.org/10.3390/s23208459) · [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/)*

| 모델 경량화 | 고령자 낙상 검출 | 고령자 일상동작 정상 판정 |
|:---:|:---:|:---:|
| **1.11 → 0.70 MB** | **13 / 15건** | **627 / 640건** |
| ResNet24 → TinyFallNet | FARSEEING · 민감도 86.67% | KFall · 특이도 97.97% |

*모델 크기는 6축 모델 비교, 고령자 결과는 3축 모델과 수정한 시간 판정의 저장 데이터 평가입니다.*

[모델별 성능표와 연구 과정 →](https://github.com/BummoK/BummoK/blob/main/projects/05-tinyfallnet.md)

### 실험실 밖의 움직임까지 생각한 연구

| 연구 | 제가 다룬 문제 | 자세히 보기 |
|---|---|---|
| **ANN·특성 선택** | 30명·23개 동작에서 32개 특성을 추출하고, 적은 특성으로 낙상을 검출하는 방법 비교 | [센서·GUI·실험 그래프](https://github.com/BummoK/BummoK/blob/main/projects/07-sensor-acquisition.md) |
| **교차 데이터셋 평가** | 연구실에서 잘 맞던 모델이 SisFall에서 달라지는 이유 분석 | [내부·외부 평가 비교](https://github.com/BummoK/BummoK/blob/main/projects/13-cross-dataset.md) |
| **건설현장 추락 예측** | 충격 전 신호로 충격 크기 예측 · 공동 제1저자 | [예측 그래프와 결과표](https://github.com/BummoK/BummoK/blob/main/projects/14-construction-fall.md) |
| **이상치 검출** | 정상 동작 학습과 미래 신호 예측으로 미관측 낙상 탐색 | [모델 구조와 실험 과정](https://github.com/BummoK/BummoK/blob/main/projects/06-anomaly-detection.md) |

![데이터셋에 따른 성능 차이](https://raw.githubusercontent.com/BummoK/BummoK/main/assets/research/cross-dataset-accuracy.svg)

*2021년 교차 데이터셋 논문 Table 3의 추가 처리 없음 조건을 재구성했습니다. [평가 조건](https://github.com/BummoK/BummoK/blob/main/projects/13-cross-dataset.md)*

[논문·학력·학회 발표 전체 보기 →](https://github.com/BummoK/BummoK/blob/main/research.md)

## 🤝 정부·기업과 함께한 연구

연세대학교 생체역학연구실에서 고령자 안전, 산업현장 보호장치, 재활 보조기기와 생체신호 기반 인터페이스 과제에 참여했습니다.

| 대표 과제 | 지원 부처·기업 | 참여 시기 |
|---|---|---|
| 착용형 로봇 사용자의 낙상 검출 | 삼성전자 용역 | 2022–2023 |
| 고소작업 추락·전도 대응 착용형 보호제품 | 산업통상자원부 | 2019–2022 |
| AI 무릎굽힘 제어형 슬관절 보조기 | 국방부 | 2021–2023 |
| 전동킥보드 탑승자용 백팩형 안전보호구 | 중소벤처기업부 | 2020–2023 |
| 고령자 낙상위험 모니터링·상해예방 | 과학기술정보통신부 | 2021–2022 |

[에어백·의수·수화 인식 등 과제 12건의 참여 이력 →](https://github.com/BummoK/BummoK/blob/main/funded-projects.md)

## 🛠️ 소프트웨어 · 연구를 직접 쓸 수 있는 도구로

센서와 모델을 다루며 반복하던 작업을 앱과 분석 도구로 만들었습니다. 개인 프로젝트에서는 화장품 탐색 서비스와 브랜드 웹사이트도 개발했습니다.

| 프로젝트 | 만든 기능 | 살펴보기 |
|---|---|---|
| **SW AIRBAG · Web / Windows / Android** | BLE 센서 연결, 실시간 차트, 기록 수집, 펌웨어 업데이트 | [화면과 개발 내용](https://github.com/BummoK/BummoK/blob/main/projects/08-sw-airbag-suite.md) |
| **Fall Trace** | 저장 기록·모델 출력·판정 이벤트의 시간축 분석 | [도구 개발 과정](https://github.com/BummoK/BummoK/blob/main/projects/09-recording-tools.md) |
| **Android 센서 AI 앱** | Kotlin·Compose 기반 BLE 수신·차트·TensorFlow Lite 추론 | [연구 앱 화면](https://github.com/BummoK/BummoK/blob/main/projects/04-android-sensor-app.md) |
| **Web App Launcher** | 모바일 앱 선택과 실행 링크 설정 | [프로젝트](https://github.com/BummoK/BummoK/blob/main/projects/10-web-launcher.md) |
| **GLOW PICK** | React·Express·MongoDB 기반 화장품 검색·리뷰 | [개인 프로젝트](https://github.com/BummoK/BummoK/blob/main/projects/11-glow-pick.md) |
| **ORIGIN I** | 반응형 브랜드 페이지와 한국어·영어 콘텐츠 | [개인 프로젝트](https://github.com/BummoK/BummoK/blob/main/projects/12-origini.md) |

| SW AIRBAG · Windows | Fall Trace · 기록 분석 |
|---|---|
| [![SW AIRBAG](https://raw.githubusercontent.com/BummoK/BummoK/main/assets/screenshots/sw-airbag-desktop.jpg)](https://github.com/BummoK/BummoK/blob/main/projects/08-sw-airbag-suite.md) | [![Fall Trace](https://raw.githubusercontent.com/BummoK/BummoK/main/assets/screenshots/recording-inspector.jpg)](https://github.com/BummoK/BummoK/blob/main/projects/09-recording-tools.md) |

| GLOW PICK · 상품 탐색 | ORIGIN I · 브랜드 웹 |
|---|---|
| [![GLOW PICK](https://raw.githubusercontent.com/BummoK/BummoK/main/assets/screenshots/glow-pick.jpg)](https://github.com/BummoK/BummoK/blob/main/projects/11-glow-pick.md) | [![ORIGIN I](https://raw.githubusercontent.com/BummoK/BummoK/main/assets/screenshots/origini-editorial.jpg)](https://github.com/BummoK/BummoK/blob/main/projects/12-origini.md) |

*센서 앱은 연결 전 화면, GLOW PICK은 테스트용 상품 화면, ORIGIN I는 브랜드 페이지 시안입니다.*

## 현재 하는 일 · 웨어러블 낙상 감지

세이프웨어에서 알고리즘 개발·평가·개선을 맡고 있습니다. 모델의 출력과 실제 움직임을 함께 살피고, 실패 사례를 찾아 수정한 뒤 같은 데이터로 다시 확인합니다.

| 업무 | 주요 경험 |
|---|---|
| [알고리즘 개발](https://github.com/BummoK/BummoK/blob/main/projects/01-sensor-ai.md) | 센서 전처리·모델 학습, AI 추정과 물리적·시계열적 움직임 특성을 종합한 판정 |
| [오류 원인 분석](https://github.com/BummoK/BummoK/blob/main/projects/02-evaluation.md) | 미검출로 보였던 2건에서 오래된 모델 출력이 평가에 사용된 원인 추적 |
| [실행 결과 비교](https://github.com/BummoK/BummoK/blob/main/projects/03-deployment-verification.md) | 5,912개 저장 시행의 Python·네이티브·DLL 재생 결과 비교 |

## 사용하는 기술

<p><img src="https://raw.githubusercontent.com/BummoK/BummoK/main/assets/badge-python.svg" alt="Python" height="30"> <img src="https://raw.githubusercontent.com/BummoK/BummoK/main/assets/badge-tensorflow.svg" alt="TensorFlow" height="30"> <img src="https://raw.githubusercontent.com/BummoK/BummoK/main/assets/badge-tflite.svg" alt="TensorFlow Lite" height="30"> <img src="https://raw.githubusercontent.com/BummoK/BummoK/main/assets/badge-numpy.svg" alt="NumPy" height="30"> <img src="https://raw.githubusercontent.com/BummoK/BummoK/main/assets/badge-pandas.svg" alt="pandas" height="30"></p>

| 분야 | 도구와 기술 |
|---|---|
| AI·신호 처리 | Python · TensorFlow/Keras · TensorFlow Lite · NumPy · pandas · SciPy · MATLAB |
| 센서·계측 | IMU · sEMG · BLE · LabVIEW · Arduino · Keil · IAR |
| 앱·웹 | Kotlin · Jetpack Compose · JavaScript · React · Express · MongoDB · Capacitor |
| 평가·데스크톱 | C/C++ · Windows DLL · PyQt · .NET · pywebview · WebView2 |

---

[koobummo726@gmail.com](mailto:koobummo726@gmail.com) · [Google Scholar](https://scholar.google.co.kr/citations?user=r-tpjqAAAAAJ) · [English](https://github.com/BummoK/BummoK/blob/main/README.en.md)

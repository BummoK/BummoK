<p align="center"><img src="https://raw.githubusercontent.com/BummoK/BummoK/main/assets/cover.png" alt="Bummo Koo — sensor AI researcher and developer" width="100%"></p>

<p align="center"><strong>Bummo Koo · PhD in Biomedical Engineering</strong><br>Algorithm Development Team Lead · Principal Researcher, Safeware</p>

<p align="center"><a href="https://github.com/BummoK/BummoK/blob/main/README.md">한국어</a> · <a href="https://github.com/BummoK/BummoK/blob/main/research.md">Research & publications</a> · <a href="https://github.com/BummoK/BummoK/blob/main/funded-projects.md">Funded projects</a></p>

## Hello 👋

I build algorithms and software that make sense of human movement. After earning my PhD at Yonsei University, I joined Safeware in May 2024. I now lead the algorithm development team, working on wearable fall detection.

My work starts with sensor data and continues through model development, evaluation and the tools people use to inspect results. I care about detecting falls early enough to help, while keeping false alarms low during everyday activities.

## 🔬 Selected research

### TinyFallNet · a smaller model for pre-impact fall detection

I developed a lightweight ResNet model and evaluated it on recorded older-adult data. This work was published in *Sensors* in 2023, with me as first author.

![TinyFallNet architecture](https://raw.githubusercontent.com/BummoK/BummoK/main/assets/research/tinyfallnet-architecture.png)

*Figure 4, Koo et al., 2023. [Paper](https://doi.org/10.3390/s23208459) · [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/).*

| Model size | Older-adult falls detected | Older-adult ADLs correctly rejected |
|:---:|:---:|:---:|
| **1.11 → 0.70 MB** | **13 / 15** | **627 / 640** |
| ResNet24 → TinyFallNet | FARSEEING · 86.67% sensitivity | KFall · 97.97% specificity |

The size comparison uses six-axis models. The older-adult evaluation uses a three-axis model with revised temporal decisions. [Architecture, results and evaluation conditions →](https://github.com/BummoK/BummoK/blob/main/projects/05-tinyfallnet.md)

| Study | What I investigated |
|---|---|
| [ANN and feature selection, 2020](https://github.com/BummoK/BummoK/blob/main/projects/07-sensor-acquisition.md) | 32 features and five ranking methods, using 23 movement types from 30 participants. First author. |
| [Cross-dataset evaluation, 2021](https://github.com/BummoK/BummoK/blob/main/projects/13-cross-dataset.md) | Why performance changes when models trained in our lab encounter SisFall movements. First author. |
| [Construction-site falls, 2022](https://github.com/BummoK/BummoK/blob/main/projects/14-construction-fall.md) | Predicting impact acceleration from pre-impact signals. Co-first author; study concept, data curation and writing. |
| [Anomaly detection, 2023](https://github.com/BummoK/BummoK/blob/main/projects/06-anomaly-detection.md) | Normal-motion training, autoencoders and future-signal prediction for unseen falls. Doctoral research. |

![Internal and external dataset accuracy](https://raw.githubusercontent.com/BummoK/BummoK/main/assets/research/cross-dataset-accuracy.svg)

*Recreated from Table 3, no-additional-processing condition, Koo et al., 2021. [Study details](https://github.com/BummoK/BummoK/blob/main/projects/13-cross-dataset.md).*

## 🤝 Government and industry research

At Yonsei's biomechanics laboratory, I contributed to projects on wearable safety, rehabilitation and biosignal interfaces. These included fall detection for **Samsung Electronics wearable robots**, **MOTIE** industrial safety systems, **Ministry of National Defense** knee orthoses, and **Ministry of SMEs and Startups** electric-scooter protection systems.

[Twelve project histories and participation periods →](https://github.com/BummoK/BummoK/blob/main/funded-projects.md)

## 🛠️ Software

| Project | What I built |
|---|---|
| [SW AIRBAG · Web / Windows / Android](https://github.com/BummoK/BummoK/blob/main/projects/08-sw-airbag-suite.md) | BLE connections, live charts, recordings and firmware-update workflows |
| [Fall Trace](https://github.com/BummoK/BummoK/blob/main/projects/09-recording-tools.md) | Tools to compare recorded signals, model outputs and detection events over time |
| [Android sensor AI app](https://github.com/BummoK/BummoK/blob/main/projects/04-android-sensor-app.md) | Kotlin/Compose app with BLE acquisition and TensorFlow Lite inference |
| [Web App Launcher](https://github.com/BummoK/BummoK/blob/main/projects/10-web-launcher.md) | Mobile app selection and launch-link settings |
| [GLOW PICK](https://github.com/BummoK/BummoK/blob/main/projects/11-glow-pick.md) | Personal React/Express/MongoDB prototype for cosmetic discovery and reviews |
| [ORIGIN I](https://github.com/BummoK/BummoK/blob/main/projects/12-origini.md) | Personal responsive brand-site prototype with Korean/English content |

| SW AIRBAG | Fall Trace |
|---|---|
| [![SW AIRBAG](https://raw.githubusercontent.com/BummoK/BummoK/main/assets/screenshots/sw-airbag-desktop.jpg)](https://github.com/BummoK/BummoK/blob/main/projects/08-sw-airbag-suite.md) | [![Fall Trace](https://raw.githubusercontent.com/BummoK/BummoK/main/assets/screenshots/recording-inspector.jpg)](https://github.com/BummoK/BummoK/blob/main/projects/09-recording-tools.md) |

| GLOW PICK | ORIGIN I |
|---|---|
| [![GLOW PICK](https://raw.githubusercontent.com/BummoK/BummoK/main/assets/screenshots/glow-pick.jpg)](https://github.com/BummoK/BummoK/blob/main/projects/11-glow-pick.md) | [![ORIGIN I](https://raw.githubusercontent.com/BummoK/BummoK/main/assets/screenshots/origini-editorial.jpg)](https://github.com/BummoK/BummoK/blob/main/projects/12-origini.md) |

*Sensor tools are shown before connection or data loading. GLOW PICK uses test products; ORIGIN I shows the brand-page prototype.*

## Current work

At Safeware, I develop wearable fall-detection algorithms and investigate false alarms, missed events and detection timing. Recent work includes [sensor AI development](https://github.com/BummoK/BummoK/blob/main/projects/01-sensor-ai.md), [tracing outdated evaluation inputs](https://github.com/BummoK/BummoK/blob/main/projects/02-evaluation.md), and [comparing Python, native and DLL replay outputs across 5,912 recorded trials](https://github.com/BummoK/BummoK/blob/main/projects/03-deployment-verification.md).

## Background and tools

- **PhD, Biomedical Engineering, Yonsei University**, 2018–2023. Dissertation: *Robust Pre- and Post-Impact Fall Detection Algorithm Based on Artificial Intelligence*.
- **Bachelor's degree, Biomedical Engineering, Yonsei University**, 2012–2018.
- **AI and signals:** Python, TensorFlow/Keras, TensorFlow Lite, NumPy, pandas, SciPy, MATLAB.
- **Sensors and software:** IMU, sEMG, LabVIEW, BLE, Kotlin, Compose, JavaScript, React, Express, MongoDB, C/C++, Capacitor and WebView2.

Detailed case studies are in Korean. [Publications and conference presentations →](https://github.com/BummoK/BummoK/blob/main/research.md)

---

[koobummo726@gmail.com](mailto:koobummo726@gmail.com) · [Google Scholar](https://scholar.google.co.kr/citations?user=r-tpjqAAAAAJ)

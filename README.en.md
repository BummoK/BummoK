<p align="center"><img src="https://raw.githubusercontent.com/BummoK/BummoK/main/assets/cover.svg" alt="Biomedical AI — Sensor algorithms, evaluation and software" width="100%"></p>

<p align="center"><strong>PhD in Biomedical Engineering · ~3 years in AI and software development</strong><br>Sensor algorithms, performance evaluation and iterative improvement</p>

<p align="center"><a href="https://github.com/BummoK/BummoK/blob/main/README.md">한국어</a> · <a href="https://github.com/BummoK/BummoK/blob/main/projects/01-sensor-ai.md">Sensor AI</a> · <a href="https://github.com/BummoK/BummoK/blob/main/projects/02-evaluation.md">Evaluation</a> · <a href="https://github.com/BummoK/BummoK/blob/main/projects/03-deployment-verification.md">Verification</a></p>

## Hello, sensor world

**I develop AI algorithms for understanding human movement.** With a research background in biomedical engineering, I have taken responsibility for algorithm development, performance evaluation and improvement in a wearable fall-detection project.

```python
background = "Biomedical Engineering, PhD"
focus = ["Sensor AI", "Wearable Healthcare"]
work = ["Develop", "Evaluate", "Improve"]
```


## Selected work

### Wearable IMU fall detection

Distinguishing falls from everyday movements while considering false alarms and detection timing. These are **three perspectives on one project**, with Korean case studies and English summaries.

<a href="https://github.com/BummoK/BummoK/blob/main/projects/01-sensor-ai.md"><img src="https://raw.githubusercontent.com/BummoK/BummoK/main/assets/case-01.svg" alt="01 Sensor AI — IMU preprocessing, model development and adaptation" width="100%"></a>

Connected sensor preprocessing, deep learning and transfer learning with decisions that combine AI estimates and physical and temporal movement characteristics.

[Explore the development approach →](https://github.com/BummoK/BummoK/blob/main/projects/01-sensor-ai.md)

<a href="https://github.com/BummoK/BummoK/blob/main/projects/02-evaluation.md"><img src="https://raw.githubusercontent.com/BummoK/BummoK/main/assets/case-02.svg" alt="02 Evaluation — Trial-level errors, timing and replay input investigation" width="100%"></a>

Analyzed trial-level errors and detection timing. The case study follows an investigation that traced apparent missed detections to outdated model outputs in replay inputs.

[Explore the evaluation and investigation →](https://github.com/BummoK/BummoK/blob/main/projects/02-evaluation.md)

<a href="https://github.com/BummoK/BummoK/blob/main/projects/03-deployment-verification.md"><img src="https://raw.githubusercontent.com/BummoK/BummoK/main/assets/case-03.svg" alt="03 Verification — Model artifacts, native execution and recorded-data replay" width="100%"></a>

Compared model artifacts and execution paths. A recorded host-replay investigation across **5,912 trials** distinguished matching decisions from differences in first-detection timing.

[Explore the comparison conditions and results →](https://github.com/BummoK/BummoK/blob/main/projects/03-deployment-verification.md)

## How I work

<img src="https://raw.githubusercontent.com/BummoK/BummoK/main/assets/workflow.svg" alt="IMU signals → model development → trial evaluation → integration checks, with an improvement loop" width="100%">

1. **Define the evaluation unit.** Separate training-window metrics from trial-level outcomes.
2. **Investigate errors over time.** Compare sensor signals, model outputs and first-detection timing.
3. **Review the trade-offs.** Assess false alarms, detection delays and regression together.
4. **Keep results traceable.** Connect input, model and decision versions with execution paths.

## My toolkit

<p><img src="https://raw.githubusercontent.com/BummoK/BummoK/main/assets/badge-python.svg" alt="Python" height="30"> <img src="https://raw.githubusercontent.com/BummoK/BummoK/main/assets/badge-tensorflow.svg" alt="TensorFlow" height="30"> <img src="https://raw.githubusercontent.com/BummoK/BummoK/main/assets/badge-tflite.svg" alt="TensorFlow Lite" height="30"> <img src="https://raw.githubusercontent.com/BummoK/BummoK/main/assets/badge-numpy.svg" alt="NumPy" height="30"> <img src="https://raw.githubusercontent.com/BummoK/BummoK/main/assets/badge-pandas.svg" alt="pandas" height="30"></p>

| Area | Technologies and methods |
|:---|:---|
| Model development | Python · TensorFlow · Keras · TensorFlow Lite |
| Sensor data and evaluation | NumPy · pandas · SciPy · IMU time series · Trial-level error analysis |
| Integration verification | C/C++ native execution comparisons · DLL replay · Algorithm integration for ARM targets |

## Interests & contact

Deep Learning · TinyML · Wearable Healthcare

Email: [koobummo726@gmail.com](mailto:koobummo726@gmail.com)

<sub>Reported comparisons use recorded data for development and regression verification. They are distinct from final device alarms and field performance; conditions are described in each case study.</sub>

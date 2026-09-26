<div align="center">

# UniFace

### Unified Face Analysis for Python

<img src="https://raw.githubusercontent.com/yakhyo/uniface/main/.github/logos/uniface_rounded_q80.webp" alt="UniFace" width="92%">

<p>
  <a href="https://yakhyo.github.io/uniface/quickstart/"><img src="https://img.shields.io/badge/Get%20Started-111827?style=for-the-badge" alt="Get Started"></a>
  <a href="https://yakhyo.github.io/uniface/"><img src="https://img.shields.io/badge/Documentation-111827?style=for-the-badge" alt="Documentation"></a>
  <a href="https://pypi.org/project/uniface/"><img src="https://img.shields.io/pypi/v/uniface.svg?style=for-the-badge&label=PyPI" alt="PyPI"></a>
  <a href="https://github.com/yakhyo/uniface"><img src="https://img.shields.io/badge/Source-upstream-111827?style=for-the-badge" alt="Upstream"></a>
</p>

</div>

---

<div align="center">

| Detection | Recognition | Tracking | Landmarks |
|---|---|---|---|
| <img src="https://raw.githubusercontent.com/yakhyo/uniface/main/assets/demo/detection.jpg" width="220"> | <img src="https://raw.githubusercontent.com/yakhyo/uniface/main/assets/demo/verification.jpg" width="220"> | <img src="https://raw.githubusercontent.com/yakhyo/uniface/main/assets/demo/face_mesh.jpg" width="220"> | <img src="https://raw.githubusercontent.com/yakhyo/uniface/main/assets/demo/landmarks.jpg" width="220"> |

</div>

<div align="center">

| Face Quality | Parsing | Matting | Gaze |
|---|---|---|---|
| <img src="https://raw.githubusercontent.com/yakhyo/uniface/main/assets/demo/quality.jpg" width="220"> | <img src="https://raw.githubusercontent.com/yakhyo/uniface/main/assets/demo/parsing.jpg" width="220"> | <img src="https://raw.githubusercontent.com/yakhyo/uniface/main/assets/demo/matting.jpg" width="220"> | <img src="https://raw.githubusercontent.com/yakhyo/uniface/main/assets/demo/gaze.jpg" width="220"> |

</div>

<div align="center">

| Head Pose | Demography | Emotion | Anti-Spoofing |
|---|---|---|---|
| <img src="https://raw.githubusercontent.com/yakhyo/uniface/main/assets/demo/headpose.jpg" width="220"> | <img src="https://raw.githubusercontent.com/yakhyo/uniface/main/assets/demo/demography.jpg" width="220"> | <img src="https://raw.githubusercontent.com/yakhyo/uniface/main/assets/demo/emotion.jpg" width="220"> | <img src="https://raw.githubusercontent.com/yakhyo/uniface/main/assets/demo/spoofing.jpg" width="220"> |

</div>

<div align="center">

| Anonymization | Segmentation |
|---|---|
| <img src="https://raw.githubusercontent.com/yakhyo/uniface/main/assets/demo/anonymization.jpg" width="330"> | <img src="https://raw.githubusercontent.com/yakhyo/uniface/main/assets/demo/segmentation.jpg" width="330"> |

</div>

---

<div align="center">

### Installation

```bash
pip install "uniface[cpu]"
```

```bash
pip install "uniface[gpu]"
```

</div>

---

<details>
<summary><b>Quick example</b></summary>

```python
import cv2
from uniface import FaceAnalyzer, FairFace

analyzer = FaceAnalyzer(predictors=[FairFace()])

for face in analyzer.analyze(cv2.imread("photo.jpg")):
    print(face.bbox, face.sex, face.age_group, face.embedding.shape)
```

</details>

---

<div align="center">

**15 face-analysis tasks**

Detection · Recognition · Tracking · Landmarks · Parsing · Matting · Gaze · Head Pose · Demographics · Emotion · Face States · Quality · Anti-Spoofing · Anonymization · Vector Search

</div>

---

<div align="center">

[Documentation](https://yakhyo.github.io/uniface/) ·
[Quickstart](https://yakhyo.github.io/uniface/quickstart/) ·
[Models](https://yakhyo.github.io/uniface/models/) ·
[Notebooks](https://yakhyo.github.io/uniface/notebooks/) ·
[Issues](https://github.com/yakhyo/uniface/issues)

</div>

<div align="center">

<sub>
This repository is a fork of <a href="https://github.com/yakhyo/uniface">yakhyo/uniface</a>.
</sub>

</div>

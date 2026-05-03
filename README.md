# CDUWD 1.0: Chengdu Urban Waterbody Semantic Segmentation Dataset

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Paper: Remote Sens.](https://img.shields.io/badge/Paper-Remote%20Sens.-blue.svg)](https://doi.org/10.3390/rs16203873)
[![Area: Chengdu](https://img.shields.io/badge/Area-Chengdu-green.svg)](https://en.wikipedia.org/wiki/Chengdu)

## 1. Introduction 📝
The **Chengdu Urban Water Body Semantic Segmentation Dataset (CDUWD)** is a high-resolution (VHR) sampleset specifically designed for urban water body extraction. 

- **Focus:** Addressing incomplete boundaries, misclassification, and omission of small water bodies.
- **Applications:** Urban planning, flood management, and ecological monitoring.
- **Compatibility:** Optimized for models like SegFormer, DeepLabV3+, and HRNet.

> [!TIP]
> This dataset supports the paper: *"Precise City-Scale Urban Water Body Semantic Segmentation and Open-Source Sample Set Construction Based on Very High-Resolution Remote Sensing: A Case Study in Chengdu"* published in **Remote Sens.**

---

## 2. Dataset Specifications 📊

| Attribute | Details |
| :--- | :--- |
| **Source Imagery** | Google Earth (Very High Resolution) |
| **Spatial Resolution** | **0.27 meters** |
| **Spectral Bands** | RGB (Red, Green, Blue) |
| **Location** | Chengdu, China |
| **Annotation** | Precise manual interpretation |

### Multi-scale Characteristics:
* **Scale Diversity:** Covers both large rivers and small urban ponds.
* **Scene Variability:** Distinct visual styles between urban core and peri-urban areas.
* **Complex Backgrounds:** High-quality labels accounting for building shadows and vegetation occlusion.

---

## 3. Composition & Classification 📁

The dataset consists of **77** source sample areas, cropped into two standardized sizes:
* **512 × 512 pixels:** 3,800 samples
* **1024 × 1024 pixels:** 950 samples

### Water Body Categories:
| Category | Type | Percentage (%) |
| :--- | :--- | :--- |
| **CDUWD-1** | Main Rivers | 20.2% |
| **CDUWD-2** | Small Rivers | 17.1% |
| **CDUWD-3** | Lakes | 30.3% |
| **CDUWD-4** | Small Water Bodies | 8.2% |
| **CDUWD-5** | Other Water | 6.0% |
| **CDUWD-6** | Non-water (Background) | 18.2% |

---

## 4. Labeling Principles 📏
- **Minimum Size:** Water bodies under 50 pixels are excluded to reduce noise.
- **Shadow Handling:** Shadows cast by buildings on water surfaces are **annotated as water** to ensure connectivity.
- **Inclusions:** Ponds, reservoirs, ditches, lakes, rivers, and wetlands.

---

## 5. Download Access 🚀

| Provider | Link | Password / Note |
| :--- | :--- | :--- |
| **Baidu Netdisk** | [Download Here](https://pan.baidu.com/s/1tQ2seau1Ilqo2RSt5ZBLqw?pwd=cdut) | `cdut` |
| **Google Drive** | [Download Here](https://drive.google.com/drive/folders/1Cf0IBprLtH44uvaNPdYILF7VYOaScwPx?usp=sharing) | - |

---

## 6. Citation 🎓
If you find this dataset useful for your research, please cite our work:

```bibtex
@article{cheng2024precise,
  title={Precise City-Scale Urban Water Body Semantic Segmentation and Open-Source Sampleset Construction Based on Very High-Resolution Remote Sensing: A Case Study in Chengdu},
  author={Cheng, Xi and Zhu, Qian and Song, Yujian and Yang, Jieyu and Wang, Tingting and Zhao, Bin and Shen, Zhanfeng},
  journal={Remote Sensing},
  volume={16},
  number={20},
  pages={3873},
  year={2024},
  publisher={MDPI}
}

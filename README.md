# CDUWD 1.0 - Chengdu Urban Waterbody Semantic Segmentation Dataset

## 1. Introduction to CDUWD 1.0

   The **Chengdu Urban Water Body Semantic Segmentation Dataset (CDUWD)** is designed to address common challenges in urban water body extraction, such as incomplete boundaries, misclassification, and omission of small water bodies. **CDUWD** focuses on improving the accuracy of urban water body extraction for applications such as urban planning, flood management, and ecological monitoring. It provides valuable training and evaluation resources for models like SegFormer, enabling efficient multi-scale urban water body segmentation in complex urban environments and is applicable to various types of urban water bodies.

   The dataset is comprehensively described in the article ***"Precise City-Scale Urban Water Body Semantic Segmentation and Open-Source Sample Set Construction Based on Very High-Resolution Remote Sensing: A Case Study in Chengdu,"*** published in **Remote Sens.,** which provides important support for future research on urban water resource management. The article is affiliated with **Chengdu University of Technology**.

## 2. Source Data

   The source data of the **CDUWD** dataset is derived from very high-resolution (VHR) images from Google Earth. There are a total of 15 images with a spatial resolution of 0.27 meters. Each image contains red, green, and blue bands, providing a rich data source for analyzing urban features such as water bodies and also serving as the basis for the generation of the CDUWD dataset.

  The water body characteristics in the CDUWD dataset demonstrate the multi-scale features and variations of urban water bodies across different areas and under complex backgrounds. Specifically, they are as follows:

1.  **Multi-scale features:** the images exhibit significant multi-scale features, portraying variations in water body spatial distribution and appearance.
2.  **Scene variability:** water bodies display contrasting styles between urban core and peripheral areas, varying from small and regular to large and irregular shapes.
3. **Complex and diverse backgrounds:** the presence of buildings and shadows complicates water body extraction, with background complexity affecting the spectral signatures and the accuracy of identification. These characteristics guided the selection of representative sample images, ensuring the dataset’s robustness for model training and analysis.

## 3. Dataset Composition and Classification

  From these Source Data, 77 sample points were selected, and 4000×4000 pixel sample images were extracted around each point. We conducted visual interpretation and precise annotation of water bodies based on a set of criteria. The annotated samples were converted into raster images and underwent cropping to create two datasets: one containing 950 samples of 1024×1024 pixels, and another containing 3800 samples of 512×512 pixels.

  Based on the distribution characteristics of water bodies in the selected samples, we constructed a new dataset, CDUWD, which is categorized into six classes:

| Subset of the dataset | Type of water body | Count | Percentage(%) |
| --- | --- | --- | --- |
| CDUWD-1 | main rivers | 192 | 20.2 |
| CDUWD-2 | small rivers | 162 | 17.1 |
| CDUWD-3 | lakes | 288 | 30.3 |
| CDUWD-4 | small water | 78 | 8.2 |
| CDUWD-5    | others water | 57 | 6.0 |
| CDUWD-6 | non-water | 173 | 18.2 |

## 4. The Labeling Principles of CDUWD

  The CDUWD dataset was obtained through precise manual annotations of the selected sample images, following these principles:

1. Water bodies under 50 pixels were not annotated.
2. Dry riverbeds, dry ditches, and channels with unclear water presence were not annotated.
3. Ponds, artificial reservoirs, water-filled ditches, lakes, rivers, visibly flooded rice fields, and wetlands were annotated. To maintain the accurate shape of extracted water bodies, shadows cast by buildings on water surfaces were also marked as water bodies.

  Annotated samples were then converted to raster images for direct use in training semantic segmentation models. A series of cropping operations were applied to these samples and annotated images, creating two datasets: one with 950 samples of 1024×1024 pixels and another with 3800 samples of 512×512 pixels.

## 5. **Download Link**

- **The dataset Water Body Dataset is shared via Baidu Netdisk:**
  
     Link: https://pan.baidu.com/s/1tQ2seau1Ilqo2RSt5ZBLqw?pwd=cdut 

     Access code: cdut
- **The dataset Water Body Dataset is shared via Google Drive：**
  
     Link: https://drive.google.com/drive/folders/1Cf0IBprLtH44uvaNPdYILF7VYOaScwPx?usp=sharing

   In the downloaded folder, there are two subfolders, named "512" and "1024". **512 folder:** Contains 3,800 samples with a resolution of 512×512 pixels, where the sample images ("images") and their corresponding labels ("labels") are stored in separate folders.**1024 folder:** Contains 950 samples with a resolution of 1024×1024 pixels. Similarly, the images and labels are stored separately in "images" and "labels" folders.Each "images" and "labels" folder is further divided into six subfolders, labeled as:CDUWD-1,CDUWD-2,CDUWD-3,CDUWD-4,CDUWD-5,CDUWD-6.Each subfolder contains the respective number of samples, annotated with different types of water bodies.

## 6. **Article citation format**

Cheng, X.; Zhu, Q.; Song, Y.; Yang, J.; Wang, T.; Zhao, B.; Shen, Z. Precise City-Scale Urban Water Body Semantic Segmentation and Open-Source Sampleset Construction Based on Very High-Resolution Remote Sensing: A Case Study in Chengdu. Remote Sens. 2024, 16, 3873. https://doi.org/10.3390/rs16203873

## 7. **Acknowledgements**

  We would like to express our sincere gratitude to Graduate Quality Engineering Construction Funding Program of Chengdu University of Technology (2024YAL016) for the support of this project.
  We also acknowledge the efforts of all contributors, whose input and collaboration greatly contributed to the success of this research.

**Chengdu University of Technology:**

Xi Cheng, Qian Zhu, Yujian Song, Jieyu Yang, Tingting Wang

**Aerospace Information Research Institute (Chinese Academy of Science) :**
Zhanfeng Shen, Haoyu Wang

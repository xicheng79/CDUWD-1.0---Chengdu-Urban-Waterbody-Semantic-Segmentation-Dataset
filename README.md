## Chengdu Urban Waterbody Semantic Segmentation Dataset (CDUWD)

### 1. Dataset Overview

This dataset is based on very high-resolution (VHR) images from Google Earth, totaling 15 images with a spatial resolution of 0.27 meters. Each image contains red, green, and blue bands, providing a rich data source for analyzing urban features such as water bodies.

### 2. Dataset Composition and Classification

From these images, 77 sample points were selected, and 4000×4000 pixel sample images were extracted around each point. We conducted visual interpretation and precise annotation of water bodies based on a set of criteria. The annotated samples were converted into raster images and underwent cropping to create two datasets: one containing 950 samples of 1024×1024 pixels, and another containing 3800 samples of 512×512 pixels.

Based on the selected sample features, we constructed a new dataset, CDUWD, which is categorized into six classes:

├──datasets code│\------------ │categories

├──CUDWD-1       │\------------ │Mainstream

├──CUDWD-2       │\------------ │Tributary

├──CUDWD-3       │\------------ │Lake

├──CUDWD-4       │\------------ │Small Waterbody

├──CUDWD-5       │\------------ │Other Waterbody

├──CUDWD-6       │\------------ │Non-Waterbody

### 3. Obtaining the CUDWD Dataset

The CUDWD dataset was obtained through precise manual annotations of the selected sample images, following these principles:

- (1) Water bodies under 50 pixels were not annotated.
- (2) Dry riverbeds, dry ditches, and channels with unclear water presence were not annotated.
- (3) Ponds, artificial reservoirs, water-filled ditches, lakes, rivers, visibly flooded rice fields, and wetlands were annotated. To maintain the accurate shape of extracted water bodies, shadows cast by buildings on water surfaces were also marked as water bodies.

Annotated samples were then converted to raster images for direct use in training semantic segmentation models. As shown in step 1 of Figure 2, a series of cropping operations were applied to these samples and annotated images, creating two datasets: one with 950 samples of 1024×1024 pixels and another with 3800 samples of 512×512 pixels.

Based on the selected sample features, we constructed the CDUWD dataset, divided into six classes: Main River Dataset (CDUWD-1), Tributary Dataset (CDUWD-2), Lake Dataset (CDUWD-3), Small Waterbody Dataset (CDUWD-4), Other Waterbody Dataset (CDUWD-5), and Non-Waterbody Dataset (CDUWD-6). This dataset allows for a refined understanding of different waterbody types in urban environments, supporting urban planning, environmental protection, and resource management. The dataset will be publicly available at [https://github.com/xicheng79/](https://github.com/xicheng79/).

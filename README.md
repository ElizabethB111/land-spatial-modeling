# EU Land Cover Spatial Modeling Project

This project focuses on building **spatial models** for European land cover classification. Using train/test splits and validation, the goal is to create models that can accurately predict land type from satellite imagery.

---

## Dataset

We use the **EuroSAT RGB dataset**, which consists of labeled satellite image patches representing different land use and land cover classes in Europe.  

- **Image size:** 64×64 pixels, RGB  
- **Classes:** 10 categories (e.g., forest, residential areas, rivers, agricultural land)  
- **Total images:** 27,000  
  - Training set: 16,200 images  
  - Validation set: 5,400 images  
  - Test set: 5,400 images  
- **Columns:**  
  1. `image` – RGB satellite tile  
  2. `label` – land use or land cover category (outcome variable)  
  3. `filename` – image identifier  

The dataset is available at: [Hugging Face EuroSAT_RGB](https://huggingface.co/datasets/blanchon/EuroSAT_RGB)

---

## Data Quality and Characteristics

- **Clean and well-structured:** No missing labels or filenames detected.  
- **Uniformity:** All images are 64×64 pixels with three RGB channels.  
- **Balanced classes:** Distribution across the ten categories is relatively even.  
- **Pixel values:** 0–255 across all channels; no clipping or normalization issues.  
- **Limitation:** Small image size, but this also improves computational efficiency for modeling.  

---

## Project Goal

Future work will involve training models on the EuroSAT RGB dataset to predict the `label` based on the `image` column. The models aim to accurately classify European land cover types using spatial patterns in satellite imagery.

---
## License
MIT License


## References

EuroSAT RGB dataset on Hugging Face https://huggingface.co/datasets/blanchon/EuroSAT_RGB

Dataset description: 64×64 RGB satellite image tiles of European land cover


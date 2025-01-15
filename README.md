## Project Title: ISIC Data Challenge
**Applications and Challenges of Multimodal Models in ISIC Melanoma Recognition**

---

## Group Members
- Shujun Jiang
- Rongrong Wang  
- Jinying Xing    
- Zhe Zhou  

---

## Course Information
**Fall 2024 Research Methods in Health Informatics and Data Visualization**

---

## Introduction
### Medical Need
- Melanoma is the deadliest skin cancer, causing over 60,000 deaths annually.
- Early detection improves survival rates up to 95%.

### Technological Opportunity
- Affordable dermatoscope attachments and smartphones enable automated image analysis.
- These tools improve access to accurate diagnoses, especially in low-resource settings.

---

## Research Questions
1. **Feature Exploration**
   - What features are linked to melanoma?
   - What features can patients provide themselves?
2. **Model Development**
   - How can image and metadata (e.g., age, gender) be combined for better diagnosis?
   - Can multimodal models outperform single-modality models?

---

## Study Design
### Methodology
1. **Data Preprocessing**
   - Dataset: ISIC Database (401,059 images).
   - Binary classification: melanoma or not.
   - Clean missing values and standardize metadata.
   - Visualize data relationships.
2. **Model Development**
   - **Image Processing:** Use Convolutional Neural Networks (CNN) for feature extraction.
   - **Metadata Analysis:** Use Random Forest to analyze variables.
3. **Evaluation**
   - Metrics: Accuracy, Recall, F1-score.
   - Feature importance analysis.
4. **Visualization**
   - Use Tableau for showcasing relationships and model outputs.

---

## Data Sources
- **Dataset:** ISIC Database
- **Size:** 401,059 dermatology images with metadata (e.g., gender, age, diagnosis).
- **Rationale for Selection:**
  - Covers diverse lesion types and metadata features.
  - High-quality annotations for reliable model development.

---

## Variables
- **Independent Variables:**
  - Image Features: Extracted via CNN.
  - Metadata Features: Gender, age, ethnicity, lesion location, etc.
- **Dependent Variables:** Binary classification (melanoma or not).
- **Covariates:**
  - Image Conditions: Lightness, resolution.
  - Health Status: Other skin conditions.

---

## Conceptual Framework
1. **Input Layer**
   - Image Data: Feature extraction via deep learning.
   - Metadata: Feature importance analysis using machine learning.
2. **Fusion Layer**
   - Dimensionality reduction with PCA.
   - Multimodal fusion using Random Forest, CatBoost, XGBoost, SVM, and MLP.
3. **Output Layer**
   - Binary classification (melanoma or not).

---

## Hypothesis
- **H₀ (Null Hypothesis):** Multimodal models do not significantly improve performance (accuracy, sensitivity, specificity, AUC) compared to unimodal models.
- **Alternative Hypothesis:** Multimodal models improve melanoma detection accuracy by integrating different data sources.

---
## Visualization
- [tableau visualization 1](https://public.tableau.com/views/ResearchMethodandDataVisualiztionFinal/OriginalDataEDA?:language=zh-CN&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link)
- [tableau visualization 2](https://public.tableau.com/views/MelanomaEDA/Dashboard1?:language=zh-CN&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link)

---

## Results
### CNN
- Final recognition accuracy: **78.73%.**
- Strength: Effective for non-melanoma cases.
- Limitation: Lower accuracy for melanoma cases.

### Random Forest
- Recognition accuracy: **94.18%.**
- Feature importance highlighted using histograms.

### CatBoost & XGBoost
- CatBoost Accuracy: **94.92%.**
- XGBoost Accuracy: **94.29%.**

### SVM
- PCA scatter plots demonstrate data consistency.
- Highlighted overlapping regions and classification challenges.

### MLP
- Achieved the highest performance: **95.03% accuracy.**

---

## Strengths
- Flexible data collection through patient-provided images and metadata.
- Improved prediction accuracy with CNN-stored features in metadata.

## Limitations
- Performance might be affected by real-world clinical differences.
- Computational resource demands limit low-resource environment application.

---

## Future Directions
1. **Hair Elimination Algorithms:** Explore their impact on image preprocessing.
2. **Dimensionality Reduction:** Investigate t-SNE for metadata processing.
3. **Model Comparison:** Introduce ResNet for a comparative study.

---

## Conclusion
- Multimodal models demonstrate superior performance over unimodal models, achieving higher accuracy, sensitivity, and specificity.
- The **CNN+MLP** combination achieved **95.03% accuracy**, proving its exceptional effectiveness in melanoma classification.

---

#### Acknowledgments

I would like to extend my heartfelt gratitude to Jinying Xing and Rongrong Wang for their invaluable contributions to this project. Their dedication, innovative ideas, and collaborative spirit greatly enriched the quality of our work. Thank you for your hard work and commitment to excellence.
# Exoplanet Detection with Machie Learning Techniques


## Overview
The **Kepler Mission**, launched by NASA in 2009 and concluded in 2018, was a pioneering effort to discover and study **exoplanets**—planets orbiting stars beyond our solar system that have the potential to support extraterrestrial life. Over the years, the Kepler telescope identified over **2,600 exoplanets**, generating an extensive dataset. With space exploration missions becoming more common, efficient methods are needed to analyze and validate exoplanetary discoveries, enhancing detection accuracy and focusing attention on the most promising candidates.

### Objective
This study aims to develop a **machine learning model** that acts as a supplementary tool for evaluating candidate exoplanets. Using a **NASA dataset**, accessible via **Kaggle**, I focused on leveraging essential features like **mass**, **radius**, and **orbital period** to classify true exoplanets versus false positives.

For further insight into data generation and processing, reference materials such as the **Kepler Data Processing Handbook** and repositories like **Caltech** and the **Mikulski Archive for Space Telescopes** are available. However, our analysis centers on the **Kaggle dataset**, exploring how machine learning techniques can refine exoplanet detection.

## Abstract

### Challenges in Exoplanet Detection
Detecting and characterizing exoplanets is challenging due to **false positives** caused by instrumental noise, stellar activity, and other astronomical phenomena.

### Objective
This study investigates various **machine learning classification methods** to distinguish genuine exoplanet candidates from false positives.

### Data Source
We use labeled data from the **NASA Exoplanets dataset**, sourced from the **Kepler Space Telescope**, to train and evaluate our models.

### Methods Compared
The study compares four machine learning techniques:
- **Support Vector Machines (SVM)**
- **Random Forest**
- **Multilayer Perceptron (MLP)**
- **XGBoost**

### Findings
All four methods demonstrate promising results, with **Random Forest** exhibiting superior performance in pattern recognition, both with and without precomputed features.

### Contribution and Future Work
This research contributes to **exoplanet detection** by suggesting that future studies could explore **deep learning methods** to improve current approaches further.

---

## Project Structure

1. **Requirements**
   - Ensure your Jupyter environment (e.g., **Google Colab**) is active.
   - Import all necessary libraries as specified in the notebook.

2. **Dataset Loading**
   - The dataset is sourced from Kaggle and can be accessed here: [NASA Exoplanet Dataset](https://www.kaggle.com/datasets/arashnic/exoplanets).
   - Upload the dataset to your Google Drive in the directory: `/content/drive/My Drive/ML/sources/exoplanets.csv`.
   - Alternatively, load the dataset directly from Kaggle using your Kaggle credentials when prompted.

3. **Execution**
   - After confirming successful data loading, proceed with the notebook, which includes the following steps:
     - **Pre-processing**
     - **Modeling**
     - **Comparison of Results**
    
## Results:
**Results Test Table:**

|    | Model                      | Accuracy | Recall                  | Precision               |
|----|----------------------------|----------|-------------------------|-------------------------|
|  0 | Random Forest               | 0.961988 | [0.95590143, 0.96984925] | [0.97615894, 0.94453507] |
|  1 | Random Forest (no KOI Score)| 0.805875 | [0.93735499, 0.64488636] | [0.7637051, 0.89370079]  |
|  2 | Multi-layer Perceptron      | 0.955409 | [0.95071336, 0.96147404] | [0.96957672, 0.9379085]  |
|  3 | MLP (no KOI Score)          | 0.807152 | [0.92111369, 0.66761364] | [0.77237354, 0.87360595] |
|  4 | SVC                         | 0.958333 | [0.95201038, 0.96649916] | [0.9734748, 0.93973941]  |
|  5 | SVC (no KOI Score)          | 0.726692 | [0.95591647, 0.44602273] | [0.67874794, 0.89204545] |
|  6 | XGBoost                     | 0.959064 | [0.96498054, 0.95142379] | [0.96248383, 0.95462185] |
|  7 | XGBoost (no KOI Score)      | 0.795658 | [0.90023202, 0.66761364] | [0.76831683, 0.84532374] |

This table provides accuracy, recall, and precision scores for each model tested. 



## Conclusion
This project aims to enhance exoplanet detection by utilizing advanced machine learning models to sift through vast amounts of space data. The results highlight the effectiveness of certain models, with **Random Forest** outperforming others. In future iterations, deeper exploration into **deep learning techniques** will be pursued to further refine detection accuracy.

---

Feel free to run the notebook in a **Jupyter environment** for optimal performance. Preferably, use **Google Colab** for seamless execution.



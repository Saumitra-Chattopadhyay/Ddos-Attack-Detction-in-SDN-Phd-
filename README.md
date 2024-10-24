# DDoS Attack Detection in SDN using Ensemble Learning Techniques

## Overview

This repository contains the implementation of ensemble machine learning models, specifically Bagging and Boosting techniques, for detecting DDoS (Distributed Denial of Service) attacks in Software-Defined Networks (SDN). The models are trained and evaluated on multiple well-known datasets, providing insights into their performance across different network environments.

## Research Overview

The primary focus of this research is to evaluate the effectiveness of ensemble learning techniques—Bagging (Random Forest) and Boosting classifiers—on detecting DDoS attacks in SDN environments. The study employs multiple datasets to ensure the models’ robustness and generalization capability. We assess the performance of these models using metrics such as accuracy, precision, recall, F1-score, and Matthews Correlation Coefficient (MCC).

### Datasets Used:
1. CICIDS2017
2. KDDCup99
3. NSL-KDD
4. Nisha Ahuja's Dataset
5. Mhd Ahmed's Dataset

## Performance Metrics
The following metrics are used to evaluate the models' performance:
- **Accuracy:** Overall correctness of the classifier.
- **Precision:** Ability to minimize false positives.
- **Recall:** Ability to detect true positives.
- **F1-Score:** Harmonic mean of precision and recall.
- **MCC:** Measures the correlation between true and predicted labels.

## Results

### Boosting Classifier

The Boosting classifier demonstrated remarkable performance across all datasets, with the highest accuracy observed on the Nisha Ahuja dataset at 99.99%, and an impressive F1-Score of 99.98%. The model maintained a balance between precision and recall, making it highly proficient in distinguishing between malicious and benign traffic.

| S.No | Dataset            | Accuracy (%) | F1-Score (%) | Recall (%) | Precision (%) | MCC    |
|------|--------------------|--------------|--------------|------------|---------------|--------|
| 1    | Mhd Ahmed Dataset   | 98.65        | 93.06        | 87.14      | 99.86         | 0.9258 |
| 2    | Nisha Ahuja         | 99.99        | 99.98        | 99.98      | 99.97         | 0.9996 |
| 3    | NSL-KDD             | 99.62        | 99.60        | 99.53      | 99.68         | 0.9976 |
| 4    | KDDCup99            | 99.98        | 99.98        | 99.98      | 99.99         | 0.9993 |
| 5    | CICIDS2017          | 99.99        | 99.99        | 99.99      | 99.99         | 0.9999 |

### Bagging (Random Forest) Classifier

The Bagging classifier also performed exceptionally well, particularly on the NSL-KDD dataset with an accuracy of 99.69% and an F1-Score of 99.81%. While not as high as Boosting on some datasets, Bagging consistently showed strong precision and recall.

| S.No | Dataset            | Accuracy (%) | F1-Score (%) | Recall (%) | Precision (%) | MCC    |
|------|--------------------|--------------|--------------|------------|---------------|--------|
| 1    | Mhd Ahmed Dataset   | 98.65        | 93.08        | 87.14      | 99.89         | 0.9260 |
| 2    | Nisha Ahuja         | 97.51        | 96.92        | 99.79      | 94.21         | 0.9503 |
| 3    | NSL-KDD             | 99.69        | 99.81        | 99.62      | 99.99         | 0.9702 |
| 4    | KDDCup99            | 99.70        | 99.81        | 99.63      | 99.98         | 0.9993 |
| 5    | CICIDS2017          | 99.94        | 99.99        | 99.90      | 99.99         | 0.9982 |

## Conclusions

The results indicate that both Boosting and Bagging classifiers are highly effective for DDoS attack detection in SDN, with Boosting slightly outperforming Bagging in most cases. These ensemble methods provide robust detection with minimal false positives and false negatives, making them viable solutions for real-world network security systems. However, the performance may vary depending on the dataset and specific network environment.

## Files Included

- **cic-ids-2017-ddos.ipynb:** Implementation on CICIDS2017 dataset.
- **kddcup99.ipynb:** Implementation on KDDCup99 dataset.
- **mhd-ahmed-dataset-notebook.ipynb:** Implementation on Mhd Ahmed's Dataset.
- **nsl-kdd.ipynb:** Implementation on NSL-KDD dataset.
- **sdn-nisha-ahuja.ipynb:** Implementation on Nisha Ahuja's dataset.

## How to Run

1. Clone the repository:
   ```bash
   git clone https://github.com/Saumitra-Chattopadhyay/Ddos-Attack-Detection-in-SDN-Phd.git
   ```
2. Install the required dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. Run the Jupyter notebooks to view the implementation for each dataset.

## Acknowledgements

This research utilizes publicly available datasets and focuses on improving DDoS detection mechanisms through advanced ensemble learning techniques.

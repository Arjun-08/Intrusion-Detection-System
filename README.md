# MACHINE LEARNING BASED INTRUSION DETECTION SYSTEM IN CLOUD COMPUTING

## Overview
Intrusion Detection Systems (IDS) are critical for maintaining the security of computer networks by monitoring and analyzing network traffic for signs of malicious activities. Traditional IDS approaches often suffer from high false alarm rates and difficulties in detecting unknown attacks. To address these issues, we implemented an IDS using the XGBoost algorithm, a powerful machine learning technique, and deployed it on AWS for scalability and efficiency. 

## Dataset
The dataset utilized in this project is the KDDcup99 dataset, a widely used benchmark dataset in the field of intrusion detection. It comprises network traffic data collected from a simulated environment containing various types of attacks and normal activities. The dataset is structured and labeled, with each data instance classified as either normal or belonging to one of several attack categories, including denial-of-service (DoS), user-to-root (U2R), remote-to-local (R2L), and probing attacks. The KDDcup99 dataset provides a comprehensive representation of network traffic scenarios, making it suitable for training and evaluating intrusion detection systems. Additionally, its size and diversity enable robust model testing and validation, ensuring reliable performance across different attack scenarios and network configurations.

## Key Features
- **High Detection Accuracy:** Achieved an accuracy of 99.17% on the KDDcup99 dataset.

  ![image](https://github.com/Arjun-08/Intrusion-Detection-System/assets/88790572/73b69939-be02-42c7-889a-4760c8ff449e)

- **Scalability:** Utilized AWS services such as Amazon S3 and Amazon SageMaker for data storage and model training.
- **Efficiency:** XGBoost's ability to handle large datasets and outliers makes it ideal for IDS applications.
- **Robustness:** Minimized overfitting by optimizing hyperparameters and validating the model rigorously.

## Results
The model achieved an impressive accuracy of 99.17% on the KDDcup99 dataset. The loss function plot indicates that the model generalizes well without overfitting, as the training and validation loss curves are close to each other.

![image](https://github.com/Arjun-08/Intrusion-Detection-System/assets/88790572/12503467-1a45-45e7-a788-86a7f76ee87d)

## Discussion

We employed XGBoost (Extreme Gradient Boosting), a robust machine learning technique, to analyze large datasets and uncover intrusion patterns within the realm of cloud computing. XGBoost operates by constructing a sequence of decision trees, each learning from the errors of its predecessor, resulting in a powerful and efficient algorithm for regression and classification tasks. Its speed, scalability, and capability to handle missing values and outliers make it ideal for processing extensive datasets. 

The implementation process involves data preprocessing, wherein relevant features are identified and data is cleaned to mitigate noise and inconsistencies. Subsequently, the data is split into training and testing sets, facilitating the creation and evaluation of decision trees. Hyperparameters such as learning rate and tree depth are optimized to enhance performance. 
Leveraging Amazon Web Services (AWS) infrastructure, particularly Amazon S3 for data storage and retrieval, and Amazon SageMaker for model development, we achieved exceptional accuracy of 99.17% on the KDDcup99 dataset. 

This success underscores the effectiveness of XGBoost in detecting potential security threats, attributed to its gradient boosting technique and regularization function. Furthermore, AWS services offer scalability, cost-effectiveness, security, and ease of use, contributing to the project's overall efficiency.

## Challenges
### Data Quality
- **Heterogeneity:** Variations in data types and structures can complicate data processing and analysis.
- **Inconsistency:** Issues like incorrect timestamps and missing data can lead to false positives/negatives in IDS.

### Class Imbalance
- **Minority Class Detection:** Techniques like oversampling, undersampling, and cost-sensitive learning are necessary to address the imbalance between normal and intrusion instances.

## Future Work
- **Enhance Feature Engineering:** Explore more advanced feature extraction techniques to improve model performance.
- **Deep Learning Models:** Investigate the use of deep learning models to automatically learn features from raw data.
- **Adaptive Systems:** Develop IDS that can adapt to new and evolving threats in real-time.


## Contact
For any questions or feedback, please open an issue in this repository or contact us at [nvarjunmani07@gmail.com](mailto:nvarjunmani07@gmail.com).

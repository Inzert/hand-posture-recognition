# Hand-Posture-Recognition
Classifying hand postures from motion capture data is a challenging problem. Measurements can vary in length due to resolution limitations of the motion capture system and posture-related self-occlusion. Additionally, the source of each measurement is usually unknown, excluding any one-to-one correspondence between records when attempting to infer hand posture from the given data. In this paper, I develop and evaluate seven classifiers with the objective of accurate classification of hand postures from unseen, real-world data. The data used for both training and testing consists of relative three-dimensional coordinates of eleven markers attached to a left-handed glove, each manually assigned to one of five classes of hand postures. The training dataset consists of 13,500 samples, while the testing dataset consists of 21,099 samples. Two of the seven classifiers presented in this paper used statistical techniques. The other five used distribution-free techniques. All classifiers were evaluated against a baseline naïve Bayes model. My results show that the best classification accuracy with respect to unseen data is attained using either linear discriminant analysis or a support vector machine with a linear kernel. This suggests that hand posture data is pairwise linearly separable in nature. This also suggests that the class conditional distributions are independent, normally distributed, and have identical covariances. Additionally, I evaluated the use of ensemble methods to improve the performance of individual classifiers by combining their best characteristics. I found that a voting classifier consisting of a support vector machine with a radial basis function kernel, a linear discriminant analysis classifier, and a quadratic discriminant analysis classifier outperformed all the individual models in testing classification accuracy.

---
File description:
- **HG_Dataset:** Contains testing and training datasets
- **Preprocessing_Feature_Selection_Model_Tuning_Code.ipynb:** Feature extraction and selection, standardization, and model tuning using cross-validation on training dataset
- **Final_Models_Evaluation.ipynb:** Evaluation of final models on testing dataset

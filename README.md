# Analyzing Diabetes Probability Using Four Different Machine Learning Algorithms
## Project information
- **Author**: Jiaolun Zhou, Computer design with track in computer science, Class of 2025, Duke Kunshan University
- **Instructor**: Prof. Luyao Zhang, Duke Kunshan University
- **Disclaimer**: Submissions to the Final Project for [Econ211 Intelligent Economy, 2023 Autumn Term (Seven Week - Second)](https://ms.pubpub.org/) instructed by Prof. Luyao Zhang at Duke Kunshan University.
- **Acknowledgments**: I extend my deepest gratitude to Prof. Luyao Zhang and classmates in Stats201 for their unwavering guidance, expertise, and encouragement, which helped me finish this project. They offered great help in giving suggestions on how to improve my work.

- **Project Summary**:

**Project Background**: As a global public health problem, the incidence of diabetes continues to rise globally, placing a heavy burden on patients' quality of life as well as on society's healthcare resources. According to the World Health Organization (WHO), approximately 422 million people worldwide suffer from diabetes, and this number is expected to grow further in the coming years. The disease not only affects the physical health of individuals, leading to a series of complications such as cardiovascular disease, nephropathy, retinopathy, etc., but also has a profound impact on the socio-economic level.

The aim of this research project is to use modern machine learning techniques to deeply mine and analyze large-scale diabetes-related data obtained from the World Health Organization, with the aim of constructing an efficient and accurate prediction model for the risk of developing diabetes. We plan to use four mainstream machine learning algorithms: support vector machine (SVM), XGBoost, linear regression, and decision tree to model and predict the likelihood of diabetes occurrence, respectively.

By comparing the performance of the different algorithms on the training and validation sets, we will select the model with the best performance as the final risk assessment tool. This model will be able to accurately predict the likelihood of an individual developing diabetes in the future based on a series of key indicators, such as blood glucose level, age, gender, body mass index, blood pressure, etc., which will provide a scientific basis for clinical decision-making and help public health policy makers and medical institutions to realize early intervention and management strategies to effectively reduce the incidence of diabetes and its complications.

**Research Questions**:

- How to apply SVM, Decision Tree, XGBoost and Linear Regression to analyze diabetes possibility?
- What factor among glucose, sex, age, fat and blood pressure affects diabetes possibility the most?
 
**AI Answer to These Two Research Questions**

<img src="7556c5104a22688c7e696f61bb15704.png" alt="Abstract Word Cloud">

<img src="d12ce9aefb9715e757a5733b57b3f3a.png" alt="Abstract Word Cloud">

  - **Project application scenarios**

1. **Clinical Decision Support System (CDSS):**
   - The model can be integrated into the electronic health record system of a medical institution to generate an individualized diabetes risk assessment report in real time based on the patient's basic biological indicators (e.g., blood glucose, blood pressure), demographic information (e.g., age, gender), and lifestyle habit data (e.g., body weight, diet, and exercise).
   - Based on this report, doctors can formulate intervention strategies in advance, such as adjusting the patient's lifestyle, guiding the rational use of medication, or arranging for more frequent monitoring to prevent the onset of diabetes.

2. **Community Health Screening and Prevention Services:**
   - The model is used to conduct rapid diabetes risk assessment for residents at community health centers or mass screening events. High-risk groups can be prioritized and recommended to attend in-depth medical checkups and receive personalized health management plans and professional guidance from dietitians, fitness trainers, and so on.

3. **Personalized health management application:**
   - Develop an intelligent health management app, whereby after users enter relevant personal information and physiological indicators, the model can provide instant feedback on their risk level for developing diabetes and suggestions for improvement.
   - The app can also integrate behavioral change incentives, such as setting health goals and tracking daily activities and eating habits, to help users reduce their risk of developing the disease.

4. **Public health policy development and resource allocation:**
   - Government and public health departments can analyze regional diabetes prevalence trends based on model predictions, allocate medical resources in a targeted manner, and design and implement preventive public health interventions, such as publicity and education campaigns on diabetes prevention and treatment, and optimizing the layout of the primary healthcare service network.

5. **Actuarial and risk management in the insurance industry:**
   - Insurance companies can apply this model to the pricing and risk assessment aspects of medical insurance products, differentiate product design and service provision based on the probability of diabetes risk of customer groups, and at the same time promote policyholders to pay attention to their own health status and take active lifestyle management measures.
  - **Research methodology**

**I. Data cleaning and pre-processing stage**

1. Data import: firstly, the original diabetes-related dataset was obtained from the WHO database.

2. Data cleaning: Remove missing values or outliers, and treat outliers appropriately. Given the needs of the project, the factor "sex" was excluded (either because it was not the main predictor variable in the setting of this study, or to test the performance of the model in the absence of gender information).

3. Data standardization or normalization: Numerical features such as blood glucose, age, BMI, blood pressure, etc. were appropriately standardized or normalized to facilitate comparison of features of different scales on the same scale.

**II. Data visualization and exploratory analysis stage**

1. Data descriptive statistical analysis: calculate the basic statistical parameters of various types of features, such as mean, standard deviation, maximum value, minimum value, etc.

2. Data visualization: drawing correlation heat map, by observing the correlation between two and two of each feature, exploring their relationship with the final result (i.e., diabetes likelihood), and searching for potential risk factors as well as multiple covariance problems.

**III. Modeling and Evaluation Stages**

1. Feature engineering: based on correlation analysis and domain knowledge, select features with significant influence to construct a feature set.

2. model training:
   a. Use XGBoost algorithm to train the model with its excellent generalization ability and good adaptability to large dataset.
   b. Construct a linear regression model for comparing the performance of non-tree-structured models.
   c. Apply Support Vector Machine (SVM) model, which is especially suitable for classification problems with small samples and high dimensionality.
   d. Build a decision tree model to visualize the importance of features and classification rules.
   
3. Model Evaluation: Divide the dataset into training set and test set, and use the cross-validation strategy to ensure the stability and robustness of the model performance. For each model, indicators such as accuracy, precision, recall, and F1 score are calculated separately, and the prediction performance of the four models is compared by these indicators.

**IV. Model Selection and Application**

1. Based on the results of model evaluation, the optimal model (i.e., the model with the highest accuracy) was selected as the main tool for diabetes risk prediction.

2. The optimal model was used to predict the test set data and its prediction effect was further analyzed, including the characteristics of misclassified samples and the potential challenges of the model in practical applications.

  - [Results]
  - [Intellectual Merits and Practical impacts of your project.]

## Table of Contents
- literature
- method
- data
- code
- results
- spotlight
- more about the author
- references

## Literature

## Method

## Data

## Code

## Result

## Spotlight
- Posters
- Figures
- Slides
- Presentations
- Review articles
- Media appearance

## More about the Author
- headshot
- self-introduction
- Final reflections 
  - intellectual growth
  - professional growth
  - living a purposeful life

## References

### Data Source
- Data Source Title and URL
### Code Source
- Code Source Title and URL
### Articles
- Article Source Title and URL
### Literature
- Literature References in [Chicago Author-Date](https://www.chicagomanualofstyle.org/tools_citationguide/citation-guide-2.html) Style and [BibTex](https://scholar.google.com/) 

Levin, Dan, and Luyao Zhang. 2020. “Bridging Level-K to Nash Equilibrium.” *The Review of Economics and Statistics* 104 (6): 1329–40. https://doi.org/10.1162/rest_a_00990.

```
@article{levin2022bridging,
  title={Bridging level-k to nash equilibrium},
  author={Levin, Dan and Zhang, Luyao},
  journal={Review of Economics and Statistics},
  volume={104},
  number={6},
  pages={1329--1340},
  year={2022},
  publisher={MIT Press One Rogers Street, Cambridge, MA 02142-1209, USA journals-info~…}
}
```


# Jiaolun_Zhou
<img src="Photo.jpg" alt="Abstract Word Cloud">

# Bio
My name is Jiaolun Zhou, from Duke Kunshan University. I am a junior student majoring in computer science. I like coding games and 3D animation, hope to be better in the future.

# Discription for this Github
This research aims to explore the use of advanced analytics and machine learning techniques to predict and manage diabetes. The study utilizes the well-known load diabetes dataset from scikit-learn and applies various statistical analyses and machine learning algorithms to uncover key features and relationships between them. The findings suggest that certain features such as age, sex, BMI, and blood pressure are important indicators of diabetes risk, while others such as S1-S6 have less impact on the disease progression. The results also demonstrate the effectiveness of XGBoost algorithm in predicting diabetes, although it requires extensive parameter tuning and computation resources. Overall, this research provides valuable insights into the complex nature of diabetes and highlights the potential of advanced analytics in improving patient outcomes.

The objective of this research is to develop a machine learning model that can accurately predict the onset of diabetes based on various physiological and demographic factors.The dependent variable (Y) is the presence or absence of diabetes, and the independent variables (X) include age, sex, BMI, blood pressure, and other biochemical markers (from s1 to s6, including glucose, obesity and other diabetes related factors).This research will use a decision tree algorithm to test our hypothesis, as it is a simple yet powerful method for classification tasks and can handle both numerical and categorical data.This research will use multiple evaluation metrics to assess the model's performance, including accuracy, precision, recall, F1 score, and area under the curve (AUC).
# Table of Contents
1. [**Self Introduction**](#self-introduction)
2. [**Data**](./Data)
   - [Data dictionary](./Data)
   - [Flowchart](./Data)
3. [**Code**](./Code)
   - [Flowchart](./Code)
# Future Research

- 1. **Integration and Comparison with Novel ML/Deep Learning Algorithms**: While the current project employs several classical machine learning algorithms, a potential avenue for future work involves incorporating state-of-the-art deep learning techniques such as Convolutional Neural Networks (CNNs), Recurrent Neural Networks (RNNs), or Generative Adversarial Networks (GANs). Moreover, integrating a broader range of machine learning models and exploring ensemble methods to further enhance prediction accuracy would be beneficial, along with comparative analysis of different model performances.

- 2. **Mathematical Logic Innovations**: Developing new mathematical reasoning frameworks could lead to the design of novel predictive models tailored specifically for diabetes risk assessment. This might involve creating unique feature extraction methods, optimizing hyperparameters using advanced optimization techniques, or devising custom regularization strategies that exploit domain-specific knowledge in a more efficient manner.

- 3. **Explainable AI (XAI) Approaches**: Given the importance of interpretability in healthcare applications, exploring explainable AI techniques to better understand the decision-making process of complex models is a critical area. This could involve implementing SHAP values, LIME, or other model-agnostic explanation methods to uncover which factors are most influential in determining diabetes risk.

- 4. **Temporal Data Analysis**: Diabetes progression is often characterized by temporal patterns. Future research could consider time-series analysis or dynamic modeling, capturing longitudinal changes in patient health data to predict not only the onset but also the progression of the disease.

- 5. **Multi-modal Feature Integration**: Combining diverse types of medical data (such as genomics, proteomics, metabolomics, and lifestyle information) within a single predictive framework can provide richer insights. Investigating how these multi-modal features can be effectively integrated and leveraged for improved diabetes prediction is another promising direction.

- 6. **Personalized Medicine**: Tailoring predictions to individual patients based on their genetic predispositions, lifestyle factors, and past medical history can significantly improve personalized care. Future studies may explore methods to refine diabetes risk prediction at an individual level.

- 7. **Causal Inference**: Moving beyond correlation, causal inference methodologies can help establish cause-and-effect relationships between risk factors and diabetes incidence. Implementing causal discovery or causal effect estimation techniques could potentially lead to actionable interventions.

- 8. **Model Robustness and Generalizability**: Ensuring that models developed are robust to variations in datasets and generalize well across different populations is essential. Research could focus on assessing and improving model performance on diverse subgroups, addressing issues related to bias, and validating models on external cohorts.

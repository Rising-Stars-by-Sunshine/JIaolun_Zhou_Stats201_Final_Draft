# Analyzing Diabetes Probability Using Four Different Machine Learning Algorithms
## Project information
- **Author**: Jiaolun Zhou, Computer design with track in computer science, Class of 2025, Duke Kunshan University
- **Instructor**: Prof. Luyao Zhang, Duke Kunshan University
- **Disclaimer**: Submissions to the Final Project for [Econ211 Intelligent Economy, 2023 Autumn Term (Seven Week - Second)](https://ms.pubpub.org/) instructed by Prof. Luyao Zhang at Duke Kunshan University.
- **Acknowledgments**: I extend my deepest gratitude to Prof. Luyao Zhang and classmates in Stats201 for their unwavering guidance, expertise, and encouragement, which helped me finish this project. They offered great help in giving suggestions on how to improve my work.

- **Project Summary**:

  - **Project Background**: As a global public health problem, the incidence of diabetes continues to rise globally, placing a heavy burden on patients' quality of life as well as on society's healthcare resources. According to the World Health Organization (WHO), approximately 422 million people worldwide suffer from diabetes, and this number is expected to grow further in the coming years. The disease not only affects the physical health of individuals, leading to a series of complications such as cardiovascular disease, nephropathy, retinopathy, etc., but also has a profound impact on the socio-economic level.
   The aim of this research project is to use modern machine learning techniques to deeply mine and analyze large-scale diabetes-related data obtained from the World Health Organization, with the aim of constructing an efficient and accurate prediction model for the risk of developing diabetes. We plan to use four mainstream machine learning algorithms: support vector machine (SVM), XGBoost, linear regression, and decision tree to model and predict the likelihood of diabetes occurrence, respectively.
   By comparing the performance of the different algorithms on the training and validation sets, we will select the model with the best performance as the final risk assessment tool. This model will be able to accurately predict the likelihood of an individual developing diabetes in the future based on a series of key indicators, such as blood glucose level, age, gender, body mass index, blood pressure, etc., which will provide a scientific basis for clinical decision-making and help public health policy makers and medical institutions to realize early intervention and management strategies to effectively reduce the incidence of diabetes and its complications.
  - [Research Questions]
 
Note: please insert the screenshot of the answers to your research question by ChatGPT. The methodology that you use to address the research questions must be more innovative than both the current literature and ChatGPT. 

  - [Application Scenario (Data Source)]
  - [Methodology]
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

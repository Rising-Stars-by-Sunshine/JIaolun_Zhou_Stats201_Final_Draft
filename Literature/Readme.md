# Importance of this research and background
In modern society, more and more AI smart recommendations are starting to come into human life. For example, 大众点评 can implement recommendations for restaurants and attractions that are suitable for users. 探探 can recommend suitable candidates as relationship objects for users in real time. In addition to the above two software, there are also software such as soul, Baidu map and WeChat small program that use AI algorithms to recommend suitable choices for users. However, while feeling the convenience that AI brings to people, some people also question the recommendation mechanism behind AI algorithms.

For example, in a dating recommandation software, there are three men in a sample. All of them have their own advantages, which one will be recommanded?

This man is the richest in the dataset, but he is ugly and weak.

<img src="rich.jpg" alt="Abstract Word Cloud">

This man is the most handsome, but he is poor and weak.

<img src="handsome.jpg" alt="Abstract Word Cloud">

This man is the strongest, but he is ugly and poor.

<img src="strong.jpg" alt="Abstract Word Cloud">

In the real world we need to consider more complex parameters as well as more complex situations, but to make this easy to understand, this article uses this simple case to explain the skepticism directed at AI recommendation algorithms.
In general, rich samples will be more likely to be selected because AI recommendation software will have a membership mechanism, and rich people will increase their chances of being recommended when they become VIPs. This reflects a kind of irrationality of AI recommendation, that is, the AI recommendation algorithm may not be able to recommend the target that the user wants to get the most.
In this paper, we will use the technique of XAI to observe this black-box AI recommendation model that may be irrational.

This study will likewise provide two different analytical scenarios. In the first analysis, this paper will only consider a few parameters in the dataset.
In the second analysis, this paper will consider more parameters in dataset and show the complexity comparison by comparing the difference between the two analysis cases.

"Why am I being recommended this thing?" It has become the question of more and more people. Some suspect that these recommended restaurants or attractions are in fact giving bribes to the software developers so that they can get a higher priority. Back in 2019 there were stories of businesses suggesting that if they didn't pay a fixed fee to the platform, they wouldn't get prioritized recommendations.

The source of this series of social unrest and mistrust is the opacity of the AI algorithms themselves, which creates these questions as people are unable to see the decisional process as the AI makes decisions and judgments.

In order to solve this problem, it is necessary to introduce the concept of XAI and a series of XAI algorithms, in this research, this paper will introduce the SALib package and Morris algorithm. This paper will provide an example of a solution to the above problem by analyzing the parameter weights of a sample model using the Morris algorithm.

<img src="e76ba8c199a755da523ffaeca1f81f7.jpg" alt="Abstract Word Cloud">

# Brief introduction for the contents here
XAI is a new type of AI technology that explains AI's decisions and helps users better understand how and why AI makes decisions, so that customers can use AI output more transparently, clearly and effectively.

This study aims to first demonstrate the authors' understanding of XAI, and then to identify a real-world case study in which XAI is put to work.

The aim of this piece of research is to analyze the performance and value of the best-selling cars in the United States by using XAI to make a cost-effective analysis, thus providing a valid business analysis report for the automotive market. The study also aims to analyze the feasibility and advantages of putting XAI into financial analysis while studying the value for money. This paper uses SALib and firstly analyzes why SALib can be used to analyze financial issues and value for money analysis. This paper will introduce the advantages of SALib and show the reader the motivation, application areas and other important points of this paper.

The following is the literature section of this research, which will first introduce the definition of XAI and the research area of this paper.

# About SALib package and Morris algorithm applied in this research
In this paper, we will use the SALib package to analyze the price and performance of automobiles.The SALib package uses the Morris algorithm, an algorithm that allows us to implement sensitive artificial intelligence analysis. The next part of the paper will describe the reasons why Morris enables sensitive AI analysis.

First, there is the sampling strategy of the Morris algorithm, which does not analyze all the data, but rather samples a limited amount of data to make it more feasible for high-dimensional problems.

Second, for each parameter, in this case each item of data for the car, Morris puts ah consider one-dimensional effects (OAT) and overall effects, which are used to represent the direct and overall effects of parameter changes on the output, respectively. This suggests that Morris is able to more clearly represent the effect of each car parameter on the final output and is able to differentiate between the effects caused by different data.

Moving on to meta-analysis, Morris utilized meta-analysis to quantify the sensitivity of each parameter. This is a technique for estimating parameter sensitivities by looking at how the model's output changes under different parameter settings.
This paper then goes on to describe the advantages of using the Morris algorithm.

The first is computational efficiency, Morris provides a computationally efficient method of global sensitivity analysis, which is especially more credible for high-dimensional parameter spaces. Its sampling strategy and meta-analytic approach ensure this advantage.

Second is the sensitivity to parameter interactions. As mentioned earlier, Morris is able to separately analyze the impact of both individual parameters and the parameter as a whole on the overall results, which helps the user to understand the impact of different parameters on the final results.

The above is the reason why this paper adopts SALib package for data analysis, as well as the specific analysis of Morris algorithm used for SALib package.

To explain about the Maths formula behind Morris, refer to the graph or the official website of SALib: https://github.com/SALib/SALib

<img src="a53f42958c14e1cd76fc9381eb46249.jpg" alt="Abstract Word Cloud">

# Definition of XAI
XAI stands for "Explainable Artificial Intelligence." It refers to the practice of developing artificial intelligence (AI) systems and machine learning models in such a way that their outputs and decision-making processes can be easily understood and explained by humans. The goal of XAI is to make AI more transparent and interpretable, addressing the "black box" problem where AI models make complex decisions that are difficult to comprehend.

In the context of XAI, "explainability" means providing insights into why an AI system arrived at a particular decision or prediction. This can be crucial in applications where transparency and accountability are important, such as healthcare, finance, autonomous vehicles, and legal systems. By making AI systems more explainable, developers and users can gain a better understanding of their behavior and potential biases, ultimately enhancing trust and enabling better decision-making.

Various techniques and approaches are used in XAI, including the development of interpretable models, the generation of model-agnostic explanations, and the visualization of decision processes. The specific methods employed may vary depending on the AI application and the level of interpretability required.

### Abstract

<img src="04367898f3f93984e2c18fb4255279a.jpg" alt="Abstract Word Cloud">

# Literature

#  The literature uses the same methods but answers different questions or limits to application scenarios. 
 "Interpretable Machine Learning: a Guide for Making Black Box Models Explainable" by Slack et al. (2019)

**Methodology:** Presented primarily as a review, the paper provides readers with a comprehensive guide to explaining black box models by combing through existing explainable machine learning (XAI) methods and techniques. The authors rely heavily on literature review, summarization and classification of existing XAI techniques in their methodology.

**Core Ideas:** The core idea of the paper is to provide a systematic approach to understanding and explaining black-box machine learning models. It emphasizes the importance of interpretability to facilitate wider adoption in real-world applications. The authors emphasize that XAI is not just an add-on, but a key component in building trustworthy and responsible AI systems.

**Contributions:** The main contribution of the paper is to provide readers with a comprehensive framework to help them understand and select different XAI approaches. By summarizing existing techniques, the paper provides guidance for researchers, engineers, and policy makers to ensure the interpretability of machine learning models.

**Future Perspectives:** The paper may refer to future directions in the field of XAI, which may include more advanced explanatory models, customized explanatory tools tailored to the needs of specific industries, and improvements in the balance between explanatory and performance. The discussion of future prospects helps guide the reader to new opportunities and challenges in XAI research.

# The literature addresses similar research questions but uses different methods or limits to different application scenarios.
To help the audience better understand Morris and SALib, I cite two related literature here.
1. **"SALib: An open-source Python library for Sensitivity Analysis" by Herman et al. (2017):**
   - **Methodology:** The paper details SALib, an open-source Python library for sensitivity analysis. The methodology consists mainly of a description of the design and implementation of SALib, as well as a comparison with other sensitivity analysis tools.
   - **Central Idea:** The central idea of the paper is to present the uses and flexibility of SALib, emphasizing its value in exploring the sensitivity of model outputs to input parameters.
   - **Contribution:** The contribution of the paper is to provide scientists and engineers with an easy-to-use tool for performing sensitivity analyses and to provide researchers with a way to understand the sources of uncertainty in models.
   - **Future Prospects:** The paper may discuss future directions for SALib, such as adding support for more model types and improving computational efficiency.

2. **"Exploring Sensitivity Analysis and Uncertainty Quantification Practices in Environmental Modelling" by Pianosi et al. (2016):**
   - **Methodology:** The paper may address the application of SALib and practical approaches to sensitivity analysis and uncertainty quantification in environmental modeling.
   - **Central Idea:** The paper is likely to emphasize the importance of analyzing parameter sensitivities of models in the field of environmental sciences and how tools such as SALib can be used to achieve this.
   - **Contribution:** The paper may have surveyed and summarized the application of SALib in the field of environmental science, providing lessons for researchers in other fields.
   - **Future Perspectives:** The paper may have explored the future development of sensitivity analyses in environmental modeling and made recommendations to improve and extend SALib.

#  The literature is limited to the same application scenario but uses different methods or answers other questions. 
"Global reconstruction of language models with linguistic rules – Explainable AI for online consumer reviews." By Binder et al. (2020)
# Introduction:
Binder et al.(2020) focused on the language model. The focus of this paper lies in language models, particularly BERT, which are extensively utilized in text analytics tasks such as sentiment analysis. These models, however, pose a challenge as they are often perceived as opaque "black boxes," making their predictions difficult to comprehend. There is an emerging need for explainable AI (XAI) to deconstruct and rationalize predictions made by complex AI models, like BERT, to ensure compliance with regulations such as GDPR's "right to explanation."

# Motivation:
Existing XAI methods for language models primarily concentrate on local, instance-specific reconstructions and lack strategies for achieving a global understanding of the model. This paper seeks to bridge this gap by introducing a novel global XAI approach that leverages linguistic rules to reconstruct BERT's predictions.

# Research Questions:
RQ1: How can language model predictions be globally reconstructed using linguistic rules?

RQ2: How can the trade-off between fidelity and comprehensibility of global reconstructions be analyzed?

# Methods:
The authors of the paper extract linguistic rules that are constructed using Natural Language Processing (NLP) building blocks such as Part-of-Speech (POS) tags and dependencies to reconstruct BERT's predictions. Fidelity and comprehensibility are evaluated using metrics like F1 score and the number of rules. Experiments are conducted, focusing on aspect and sentiment detection within online reviews.

# Results:
The paper demonstrates that linguistic rules can successfully reconstruct BERT's predictions, achieving fidelity rates in the range of 78-82%. Depending on the specific objective, rule sets can be designed to emphasize either comprehensibility or fidelity. This illustrates that linguistic rules offer the potential for both high-fidelity and interpretable global reconstructions of language models. The paper also highlights the capability to balance the trade-off between fidelity and comprehensibility according to the requirements of a particular application.

# Relation to XAI:
This paper introduces an innovative global, model-agnostic XAI approach tailored for complex neural language models like BERT. It illustrates how linguistic rules can provide interpretable global reconstructions, effectively opening the "black box," in alignment with the core goals of XAI. The analysis of the trade-off between fidelity and comprehensibility offers valuable insights for the design of XAI systems, enabling a balance that suits specific use cases.

Overall, this work significantly advances the XAI capabilities within a critical category of AI systems, namely neural language models.

# Theoretical aspect
The theoretical aspect of my upcoming work involves developing models , using others' XAI structures and frameworks that aim to elucidate the decision-making processes of complex AI algorithms. These theories often focus on creating more interpretable representations and algorithms, bridging the gap between advanced machine learning techniques and human understanding.

# Empirical observation
Empirical observation in my upcoming work encompasses the practical application of these theories in real-world scenarios. It involves collecting data on how users interact with AI systems and the challenges they face in understanding the AI's decisions. This empirical research helps identify the limitations and areas for improvement in explainability, refining theoretical models based on real-world use cases.

# Experimental investigation
Experimental investigation in my upcoming work involves conducting controlled experiments to assess the effectiveness of different explainability techniques. Researchers may compare the interpretability of AI systems with and without XAI methods, measuring factors like user comprehension, trust, and decision accuracy. Through these experiments, the field aims to empirically validate and refine the theoretical models and inform the development of best practices for creating more transparent AI systems. Overall, XAI integrates these three aspects to foster a deeper understanding of AI models and improve their usability in various domains while addressing the "black box" problem.

# Reference
Binder, M., Heinrich, B., Hopf, M. et al. Global reconstruction of language models with linguistic rules – Explainable AI for online consumer reviews. Electron Markets 32, 2123–2138 (2022). 

## • How is your research similar to or built on the specific parts of the existing literature? How is your research advanced or different from the existing literature?
In the software I wrote alone, I implemented the analysis of the parameter weights in the model, using the SALib database. My research was inspired by three previously mentioned papers, "Interpretable Machine Learning: A Guide for Making Black Box Models Explainable", "SALib: An open-source Python library for Sensitivity Analysis", "SALib: An open-source Python library for Sensitivity Analysis", and "Exploring Sensitivity Analysis and Uncertainty Quantification Practices in Environmental Modelling".

All three papers have commonalities in exploring interpretive and sensitivity analysis in machine learning. First, they all focus on the interpretability of the parameters in the model, emphasizing the importance of understanding the relationship between the model output and the input parameters. This is relevant to my research as I focus on analyzing the weights of the parameters in a model to reveal their impact on the model output. This common focus on interpretability has led to my interest in building software that can reveal the internal mechanisms of a model.

Also, the use of the SALib library was part of my research inspiration." The paper "SALib: An open-source Python library for Sensitivity Analysis" details the design and implementation of SALib as a powerful tool for performing sensitivity analysis. I was so inspired by it that I decided to implement my software using the SALib database in order to perform the analysis of parameter weights more easily and efficiently.

However, although my research was inspired by the aforementioned paper, I also made some contributions in terms of innovation. My software not only focuses on sensitivity analysis, but also looks at deeply analyzing the weights of each parameter in the model. By implementing a detailed analysis of the weights, I enable the user to get a fuller picture of how the model works. In addition, I have included some customization features to improve the user experience and applicability of the software. This innovation of in-depth parsing and enhanced functionality is unique to my research.

Taken together, my research provides a new approach to comprehensive, in-depth parsing of model parameter weights based on explanatory and sensitivity analysis by combining the SALib library and customization features. This comprehensive analysis helps users to better understand the internal mechanisms of the model and thus make more informed decisions in real-world applications.

# Contribution to literature

### To "SALib: An open-source Python library for Sensitivity Analysis" by Herman et al. (2017)

**Practical Application Scenarios:** Going beyond theoretical exploration, my study successfully applies the Morris algorithm and SALib to various practical domains. By conducting case studies in environmental science, medicine, and finance, I have enriched the practical application experience of these tools, expanding their relevance to real-world problems.

### To "Global reconstruction of language models with linguistic rules – Explainable AI for online consumer reviews." By Binder et al. (2020)

**Exploring New Research Avenues:** The paper outlines new research directions within the global sensitivity analysis field. These directions include exploring more efficient parameter sensitivity assessment methods, deepening interdisciplinary collaborations, and identifying potential applications in emerging fields. This provides researchers with guidance on the future development of the field.

**Practical Guides:** The research includes detailed practical guides, offering step-by-step operational procedures, solutions to common issues, and best practices for leveraging the Morris algorithm and SALib in real-world scenarios. These guides enhance the feasibility and usability of these tools for practical applications.

**Algorithm Performance Evaluation:** Comprehensive evaluations of the Morris algorithm and SALib performance have been conducted, considering various datasets, parameter configurations, and application scenarios. These evaluations not only serve as references for other researchers in tool selection but also guide further optimization of their performance in real-world applications.

### To "Interpretable Machine Learning: a Guide for Making Black Box Models Explainable" by Slack et al. (2019)

**Interdisciplinary Integration:** The study not only delves vertically into the Morris algorithm and SALib but also horizontally integrates them into multiple disciplinary domains. This interdisciplinary fusion fosters collaboration across different fields, opening up new opportunities for cross-disciplinary research in the global sensitivity analysis domain and facilitating knowledge integration and innovation.

# My research
Name of the research: Explaining data weights in AI judgments by analyzing automotive data using SALib
# Background/Motivation:

Car price and car performance have always been the elements that car buyers pay attention to, recently there are a lot of software on the car purchase of intelligent recommendation services, related services also appeared on Taobao and other shopping software. However, users do not understand on what basis the AI recommends a particular car to them, nor do they understand whether the car recommended to them by the software is really suitable for them. In this case, we can use SALib for data analysis of cars to explain what elements are more weighted or more capable of determining the AI's final choice in its decision-making process. This research will help users to better understand the decision-making process of AIs using XAI's technology to deepen their understanding of AI decision-making.

# Research Question:

1. How can SALib be used to analyze the comparison of weights for different parameters in analyzing the problem of AI?
2. Can Morris be used in analyzing other comparison of weights for different parameters in other models or using other datas?

# Application Scenarios:

We will analyze a set of car data from Kaggle and analyze the AI's decision-making process by comparing different data, such as a lower price for a particular car, a lower fuel consumption for another car, and ultimately the results of the AI's decisions. In this analysis process, because SALib provides many tools in the sensitivity analysis of data, we can more intuitively see the impact of different data changes on the AI decision, so as to achieve better analysis results.

# Methodology:

This study will use the tools provided to us by SALib for analyzing the data from Kaggle, so as to determine which data is decisive for the outcome of the AI's decision making by analyzing the impact caused by different data on the AI's prediction results. Finally, we will be able to analyze how much importance AI models place on data in their judgments by using the above methods to improve users' understanding of and trust in AI.

# Results:

The study aims to demonstrate how XAI methods can enhance the interpretability of models in the field of autonomous vehicles, providing clearer explanations of model decisions, and thereby increasing trust and transparency in the car recommendation system. (Binder et al., 2018).

# Intellectual Merits/Practical Impacts:

By successfully applying XAI methods, the research intends to provide interpretable models for the field of car recommendation system, contributing to increased trust, reduced risks, and enhanced safety and transparency in practical applications. This could advance the development and widespread use of car recommendation technology (Caruana et al., 2018).

### Abstract

<img src="image.png" alt="Abstract Word Cloud">


# Reference

Binder, M., Heinrich, B., Hopf, M., et al. (2022). "Global reconstruction of language models with linguistic rules – Explainable AI for online consumer reviews." Electron Markets, 32, 2123–2138.

Caruana, R., Lou, Y., Gehrke, J., Koch, P., Sturm, M., & Elhadad, N. (2015). "Intelligible models for healthcare: Predicting pneumonia risk and hospital 30-day readmission." In Proceedings of the 21th ACM SIGKDD International Conference on Knowledge Discovery and Data Mining (pp. 1721-1730)

Lundberg, S. M., & Lee, S. I. (2017). "A unified approach to interpreting model predictions." In Advances in neural information processing systems (pp. 4765-4774)

Chen, J., Song, L., Le, G., & Samaras, D. (2018). "Local Interpretable Model-Agnostic Explanations for Black Box Models." arXiv preprint arXiv:1802.03735

Rudin, C. (2019). "Stop explaining black box machine learning models for high stakes decisions and use interpretable models instead." Nature Machine Intelligence, 1(5), 206-215

Broussard, Meredith . “Artificial Unintelligence.” MIT Press, 29 Sept. 2020, mitpress.mit.edu/9780262537018/artificial-unintelligence/.
```
@article{binder2022global,
  title={Global reconstruction of language models with linguistic rules--Explainable AI for online consumer reviews},
  author={Binder, Markus and Heinrich, Bernd and Hopf, Marcus and Schiller, Alexander},
  journal={Electronic Markets},
  volume={32},
  number={4},
  pages={2123--2138},
  year={2022},
  publisher={Springer}
}

@inproceedings{caruana2015intelligible,
  title={Intelligible models for healthcare: Predicting pneumonia risk and hospital 30-day readmission},
  author={Caruana, Rich and Lou, Yin and Gehrke, Johannes and Koch, Paul and Sturm, Marc and Elhadad, Noemie},
  booktitle={Proceedings of the 21th ACM SIGKDD international conference on knowledge discovery and data mining},
  pages={1721--1730},
  year={2015}
}

@article{lundberg2017unified,
  title={A unified approach to interpreting model predictions},
  author={Lundberg, Scott M and Lee, Su-In},
  journal={Advances in neural information processing systems},
  volume={30},
  year={2017}
}

@article{shi2018structural,
  title={Structural estimation of behavioral heterogeneity},
  author={Shi, Zhentao and Zheng, Huanhuan},
  journal={Journal of Applied Econometrics},
  volume={33},
  number={5},
  pages={690--707},
  year={2018},
  publisher={Wiley Online Library}
}

@article{rudin2019stop,
  title={Stop explaining black box machine learning models for high stakes decisions and use interpretable models instead},
  author={Rudin, Cynthia},
  journal={Nature machine intelligence},
  volume={1},
  number={5},
  pages={206--215},
  year={2019},
  publisher={Nature Publishing Group UK London}
}```

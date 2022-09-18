# ML-for-Solubility-Prediction

This Repository contains the Dissertation on the topic of "Machine Learning for Solubility Prediction of Chemical Compounds". 

## Abstract 
Solubility Prediction of chemical compounds using Machine Learning has been an area of great discussion and research for the last few decades. It remains a very challenging task because measuring Solubility is a complex procedure, and the measured Solubility data is always expected to have some experimental errors. Finding a suitable Machine Learning algorithm has also been challenging, considering the unavoidable errors in experimental data and lack of relevant data.

In this research, we considered features that are most relevant for measuring the Solubility of a chemical compound. We built many conceptually different Machine Learning algorithms and focused on finding the most pertinent algorithms for the job. We also devise a way to acknowledge unavoidable errors in experimental data when assessing these models. Finally, we combined the predictions of the top-performing Machine Learning models for a final prediction. This research shows how better predictions are possible if 1. Only relevant data is considered 2. Models are assessed considering the unavoidable experimental errors, and 3. A consensus of best-performing models is taken for the final prediction. The file **"Dissertation.pdf"** will cover the theory and results of the project.  
## Machine Learning methods used

This dissertation aims to present work from the side of developing and employing relevant machine learning algorithms. We focus on building various models, aiming to cover most of the present-day machine algorithms. For this purpose, we divide our models into five different approaches, as can be seen below:

**1. Ordinary Linear Regression approaches**

• Ordinary Least Squares
• Ridge Regression
• Lasso Regression
• Support Vector Regression

2. Latent-variable approaches

• Principle components regression
• Partial least squares

3. Ensemble Learning approaches

a. Bagging algorithms

• Bagging of Decision trees
• Random forest
• Extremely randomised trees 

b. Boosting algorithms

• Adaptive boosting • Gradient boosting

4. Kernel-based approaches

• Non-linear Support Vector Regression
• Gaussian Processes

5. Artificial Neural Networks approach

• Multi-layer perceptron algorithm.

## Information about the Jupyter Notebooks

MAIN.ipynb = It is the notebook which contains the actual work that was done to get the outputs and results.

All-Features.ipynb = This notebook shows a special case where no features were dropped as part of data cleaning and even highly correlated features were considered for modeling.

G_sol, volume and SASA Removed.ipynb = This notebook contains a special case where features "G_sol", "volume" and "SASA" were removed.

In the MAIN.ipynb as a part of data understanding and cleaning, we remove "G_sol" and "volume" because of their very high correlation with other features. The other two notebooks are kept to show the following:

1. How final prediction performance drops if these features are not dropped, in All-Features.ipynb

2. How final prediction performance drops if 'SASA' is dropped because of its high correlation along with "G_sol" and "volume", in G_sol, volume and SASA Removed.ipynb.

We finally conclude that "G_sol" and "volume" should be the only features that should be dropped. As for "SASA", even though it has some high correlation should still be retained in the dataset because it seems to carry some necessary independent information for the models.

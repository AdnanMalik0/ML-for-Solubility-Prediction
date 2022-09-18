# ML-for-Solubility-Prediction

## The files for the Dissertation work on 'Machine Learning for Solubility Prediction' are kept in this Repository.

MAIN.ipynb = It is the notebook which contains the actual work that was done to get the outputs and results.

All-Features.ipynb = This notebook shows a special case where no features were dropped as part of data cleaning and even highly correlated features were considered for modeling.

G_sol, volume and SASA Removed.ipynb = This notebook contains a special case where features "G_sol", "volume" and "SASA" were removed.

In the MAIN.ipynb as a part of data understanding and cleaning, we remove "G_sol" and "volume" because of their very high correlation with other features. The other two notebooks are kept to show the following:

1. How final prediction performance drops if these features are not dropped, in All-Features.ipynb

2. How final prediction performance drops if 'SASA' is dropped because of its high correlation along with "G_sol" and "volume", in G_sol, volume and SASA Removed.ipynb.

We finally conclude that "G_sol" and "volume" should be the only features that should be dropped. As for "SASA", even though it has some high correlation should still be retained in the dataset because it seems to carry some necessary independent information for the models.

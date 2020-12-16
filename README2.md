Workflow

The dataset had a lot of missing values and noisy data. This was initally a regression problem , predicting Salary based on scores.
I tried fitting a regression model only to see an R2 value of 0.27 with little scope of improvement.
Therefore I created a new column called Salary Class based on a threshold of Salary - 3Lakhs.
If salary is above threshold - 1 else 0.

After data preprocessing , I applied various classification models , maximum accuracy around 70 percent for Logistic Regression with almost similar precision and recall.
For exploratory purposes - I increased the threshold to 6lakhs  , created a data imbalance of 24:1 . Applied classification models again only to realize
the precision and recall for minority class were below acceptance rates.

I applied Oversampling and Smote tehcniques on the dataset whihc improved both precision and Recall. This model can be used in real world practical data analysis.

For further exploration - I applied Unsupervized Learning on the initial dataset containing Salary.
KMeans showed an elbow at n=2. Using those labels Classification Models were applied and Modesls showed a lot of improvements - but that can be due to overfitting on the actual data.
The clusters were not homogeneously seperated so i applied PCA , first 20 components explained 95% of variability.
After Applying PCA - clusters were more homogeneous than before , also model metrics had improved.

EDA is done in the file Capstone File - Dropped Features.
ALL base models and Oversampling Techniques applied in Base Model File.
USL and PCA applied in the last file.

I have also uploaded the initial dataset labelled as train.xlsx along with the data description.

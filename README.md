# Cancer-RNA-Seq-Logistic-Regression
##Q1. What is the objective of this project?

###A. The objective is to classify different cancer types using RNA-seq gene expression data by applying multiclass logistic regression.

##Q2. What type of data is used in this project?

###A. Publicly available cancer RNA-seq gene expression data from Kaggle, where each sample represents a tumor and each feature represents a gene’s expression level.

##Q3. What is the machine learning task here?

###A. Multiclass classification, where the goal is to predict the cancer type (e.g., BRCA, LUAD, PRAD) for each sample.

##Q4. Why did you choose logistic regression?

###A. Logistic regression is interpretable, handles high-dimensional data well with regularization, and provides probabilistic outputs, which are suitable for biological classification problems.

##Q5. How did you preprocess the data?

###A.Merged gene expression data with cancer labels using sample IDs. Performed stratified train–test split. Scaled gene expression features using statistics learned only from the training data to avoid data leakage

##Q6. Which model configuration was used?

###A. Multiclass logistic regression trained using the SAGA solver with increased maximum iterations to ensure convergence on high-dimensional RNA-seq data.

##Q7. How was the model evaluated?

###A.
Train and test accuracy

Classification report (precision, recall, F1-score per cancer type)

5-fold stratified cross-validation

##Q8. What were the results?

###A.
Test accuracy: ~100%

Mean cross-validation accuracy: ~99.8%
These results indicate strong separability of cancer types based on gene expression profiles.

##Q9. How do you interpret the model biologically?

###A. Logistic regression coefficients can be examined to identify genes that contribute most strongly to distinguishing specific cancer types.

##Q10. What are the limitations of this project?

###A.

No external dataset validation

Batch effects were not explicitly corrected

Results should not be interpreted as clinically deployable

##Q11. What future improvements can be made?

###A.

Validation on independent cohorts

Batch-effect correction

Pathway-level biological interpretation of top genes

# Description
A lot has been said during the past several years about how precision medicine and, more concretely, how genetic testing is going to disrupt the way diseases like cancer are treated. Once sequenced, a cancer tumor can have thousands of genetic mutations. But the challenge is distinguishing the mutations that contribute to tumor growth (drivers) from the neutral mutations (passengers). As not all mutations lead to cancer. Due to a mutation in a gene, there is some genetic variation developed in a gene. But the question comes, from which particular mutation this genetic variation happened in a gene. Currently this interpretation of genetic mutations is being done manually which is a very time-consuming task. Based on a gene and a variation in it, a clinical pathologist has to manually review and classify every single genetic mutation based on evidence from text-based clinical literature.

# Real-world/Business objectives and constraints
- No low-latency requirement. 
- Interpretability is important. 
- Errors can be very costly.
- Probability of a data-point belonging to each class is needed.

# Source 
https://www.kaggle.com/c/msk-redefining-cancer-treatment/

# Performance Metric
- Multi class log-loss
- Confusion matrix

# File Descriptions
**TrainingData** - a comma separated file containing the description of the genetic mutations used for training. Fields are ID (the id of the row used to link the mutation to the clinical evidence), Gene (the gene where this genetic mutation is located), Variation (the aminoacid change for this mutations), Class (1-9 the class this genetic mutation has been classified on)

**TrainingText** - a double pipe (||) delimited file that contains the clinical evidence (text) used to classify genetic mutations. Fields are ID (the id of the row used to link the clinical evidence to the genetic mutation), Text (the clinical evidence used to classify the genetic mutation)

# Conclusion 

![Screenshot (14)](https://user-images.githubusercontent.com/42304018/72015341-98938580-3287-11ea-93e6-08e862496d0d.png)
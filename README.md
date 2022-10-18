# Handwritten-Digits
Machine Learning Application with R (Random Forest, XGBoost, Neural Network/Multiplayer Perception[MLP])

Executive Summary (All visuals will be shown in the PDF file)
[Correctly Identify Handwritten Digits.pdf](https://github.com/EvanaZhang/Handwritten-Digits/files/9805270/Correctly.Identify.Handwritten.Digits.pdf)


Business Problem & Objectives

This project’s objective is to correctly identify digits from a dataset of tens of thousands of handwritten images by developing neural network(multilayer perception), XGBoost, and random forest models.


Model Performance Summary & Interpretation

This dataset has total 786 pixels in each digit. The first step is check dataset profile by using skim() function, and then scaled each pixel before building models. Prior to splitting the dataset into training and testing dataset, a level of 3 k-fold cross-validation will be assigned to the dataset.
  
      XGBoost Modeling
      
      • Tune the parameter of 2 with 10 different sizes: tree_depth, min_n, learning rate
      
      Random Forest Modeling
      
      • Randomly tuned 2 parameters to a total of 10 different size: tree values with a range of 390 to 400 and min_n with no range.
      
      Multilayer Perception Modeling
      
      • Tuned 3 parameters with 3 different sizes: epoch with a range between 1 to 20, penalty, and hidden_units
      

Conclusion
      
• Tree depth determines the depth of the trees; the min_n indicates the minimum number of variables and the learning rate manifests the coefficient when tuning.
• Epoch indicates the number of times the dataset passes the model; penalty decides the model’s loss function; hidden units control the number of functions for the model’s input.
• By comparing the ROC_AUC and the accuracy from the Multilayer Perception, XGBoost and Random Forest models. Random forest model will be the best model to fit the data. That’s why using the random forest model to do the kaggle prediction with the highest values on both accuracy and roc_auc. (See Detailed Analysis and Steps Table 4)



      
      
      
      
      
      

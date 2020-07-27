# Arya assignment

Last column of the csv is the one that needed to be predicted, since it have binary values so it is a classification problem,
there are many classification algorithms that can be utilised such as Random Forest, SVM, KNN and lot of others.

A simple analysis reveals standard deviation varies across column but so does the max and min range as a result manual selection of features is not possible.

After plotting a chart for several columns (ONE AT A TIME), we realise this is a highly cleaned dataset with no missing values and little to no outliers. As a result, not much data preprocessing is required.

Since Number of classes are just 2 but the independent columns are 57 in number, it is apparent that KNN will not be the best solution.

so we proceed with SVM and random forest.

Upon application it is found out that random forest offered better validation accuracy then SVM (although SVM had 99% training accuracy as compared 88% of random forest).

Further, we tried to test that manual feature reduction is not possible so will it do any better on automatic feature reduction. Hence we applied PCA for same.
Upon application of PCA for various values of Ncomponents several point drops in accuracy were observed.

Based on above experience, following are the conclusions

1) 'Results.csv' contains predictions for test_set.csv
2)  Principal Component Analysis reduced the accuracy of model
3)  Random forest turned out to be the best model
4)  High Training accuracy doesnt necessarily translates to high test accuracy

Here is the [link](https://github.com/SamanthaHGerber/practicalapplication3/blob/main/prompt_III.ipynb) to my code accompanied with graphs, models, and analysis. 

The data used is a banking marketing dataset from UC Irvine which can be found [here](https://archive.ics.uci.edu/dataset/222/bank+marketing).

This [link](https://mo-pcco.s3.us-east-1.amazonaws.com/BH-PCMLAI/module_17/module_17_starter.zip) provides more information about the dataset and features. 

The process I took to complete this project:
1. Read the data
2. Underestand the features
3. Clean data
4. Engineer features
5. Train/test split
6. Create baseline models (Random, Most Frequent)
7. Build a Logistic Regression model
8. Score model
9. Initialize and create KNN, Decision Tree, SVM
10. Compare results and performance
11. Document Obervsations (see below)
12. Brainstorm next steps and recommendations (see below)

Observations:

The training time is shortest for KNN at 0.012. The Decision Tree model took almost 20x longer to train than KNN at 0.219. The SVM took 2000x longer to train than KNN or 100x longer than the Decision Tree model at 24.739. SVM takes significantly longer than the other models.
The Decision Tree model has the highest training accuracy of 1.000. The SVM was next with training accuracy of 0.927. Lastly the KNN had the lowest training accuracy at 0.899. All three have pretty high training accuracies.
The SVM has the high test accuracy at 0.914. This is followed by KNN with a test accuracy of 0.901. The Decision Tree has the lowest training accuracy but not by much of 0.895.
The Decision Tree model has the highest AUC (0.737) followed by SVM (0.695), and KNN (0.592).
The Decision Tree model has the highest Recall (0.533) followed by SVM (0.413) and KNN (0.193).
The KNN model has the highest precision (0.737) followed by SVM (0.705) and Decision Tree (0.533).
The KNN has the highest specificity (0.991) followed by SVM (0.978) and Decision Tree (0.941).
All three models (KNN, Decision Tree, SVM) have the same prevalence of 0.113.
The Decision Tree has the highest F1 score (0.533) followed by SVM (0.521) and KNN (0.316).
Our baseline models are Most Frequent and Random. Random actually performed better (3x) or the same (1x) than Most Frequent that performed better (1x) and the same (1x).

Next Steps and Recommendations:

Train more models such as Random Forest and Guassian Naive Bayes. This project focused on four models (Linear Regression, KNN, Decision Tree, and SVM), but exploring additional models could produce additional results.
Explore addional feature engineering to take out certain features or change the way nulls are replaced. We can also treat encodings differently, for example the 999 values.
We could quantify the cost of a campaign and the gain of a successful deposit. How much does it cost when customers deposit incorrectly or they are misclassified? How much does it benefit the bank when the deposits are successfully classfied and deposited?

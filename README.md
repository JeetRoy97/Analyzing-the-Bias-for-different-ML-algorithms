# Analyzing-the-Bias-for-different-ML-algorithms
Dataset: Download the UTK Face dataset from the this link. You may resize the images to 64 x 64
Algorithm: Perform classification using:
1. LCNN model (9 Conv layer version)
2. Linear SVM
Testing: Test the model on gender attribute for different race and age category. You can consider Age (0
-28 ) as children , (28-56) as Young , (56-84) as Adults and (84-116) as Old. You need to report the gender
prediction across all the four race groups and all the 4 age groups.
Evaluation Perform a 2-class classification and report the performance as follows:
1. Testing performance across all the age groups and race categories.
The dataset is divided into train:valid:test split of 70:20:10 = 16595:4741:2369
samples.
1. Testing performance across all the age groups and race categories.

![Aspose Words 50618ed9-b1b2-4630-9df0-4f841fa4401b 001](https://user-images.githubusercontent.com/59523992/163758014-e04e3c04-6d3a-4475-82b1-1ef6825beee7.png)

Figure 1: SVM age-wise accuracy

![Aspose Words 50618ed9-b1b2-4630-9df0-4f841fa4401b 002](https://user-images.githubusercontent.com/59523992/163758084-28397cb7-9046-4006-ae27-adf47529054e.png)

Figure 2: LCNN age-wise accuracy

![Aspose Words 50618ed9-b1b2-4630-9df0-4f841fa4401b 003](https://user-images.githubusercontent.com/59523992/163758100-f4834310-b8b1-49f6-a264-7dbfbbe8ea17.png)

Figure 3: LCNN age-wise accuracy at focal loss


3. ROC curve for SVM and LCNN for gender prediction tasks. (Draw ROC curve from scratch.)
4. Draw the Precision-Recall curve. (Draw Precision-Recall curve from scratch.)
5. Of the two curves stated above, which is more reliable for biased/imbalanced data? Why? Draw
inferences from the observed results on why one approach (SVM or LCNN) performs worse/better than
the other.
5. Do You observe any bias in the data ? Analyze the results.
6. Change the loss function to focal loss for LCNN. Now compare the results with previous loss function
that you have used ?

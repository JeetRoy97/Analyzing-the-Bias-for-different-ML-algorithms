# Analyzing-the-Bias-for-different-ML-algorithms
Dataset: Download the UTK Face dataset from the this link. You may resize the images to 64 x 64
Algorithm: Perform classification using:
1. LCNN model (9 Conv layer version)
2. Linear SVM
Testing: Test the model on gender attribute for different race and age category. You can consider Age (0
-28 ) as children , (28-56) as Young , (56-84) as Adults and (84-116) as Old. You need to report the gender
prediction across all the four race groups and all the 4 age groups.

Evaluation Perform a 2-class classification and report the performance as follows:

a) Testing performance across all the age groups and race categories.
Results - The dataset is divided into train:valid:test split of 70:20:10 = 16595:4741:2369
samples.
Testing performance across all the age groups and race categories.

![Aspose Words 50618ed9-b1b2-4630-9df0-4f841fa4401b 001](https://user-images.githubusercontent.com/59523992/163758014-e04e3c04-6d3a-4475-82b1-1ef6825beee7.png)

Figure 1: SVM age-wise accuracy

![Aspose Words 50618ed9-b1b2-4630-9df0-4f841fa4401b 002](https://user-images.githubusercontent.com/59523992/163758084-28397cb7-9046-4006-ae27-adf47529054e.png)

Figure 2: LCNN age-wise accuracy

![Aspose Words 50618ed9-b1b2-4630-9df0-4f841fa4401b 003](https://user-images.githubusercontent.com/59523992/163758100-f4834310-b8b1-49f6-a264-7dbfbbe8ea17.png)

Figure 3: LCNN age-wise accuracy at focal loss

![Aspose Words 50618ed9-b1b2-4630-9df0-4f841fa4401b 004](https://user-images.githubusercontent.com/59523992/163758287-9bb05584-b48c-45df-aeb5-dbe8780dc9d5.png)

Figure 4: SVM race-wise accuracy

![Aspose Words 50618ed9-b1b2-4630-9df0-4f841fa4401b 005](https://user-images.githubusercontent.com/59523992/163758300-d685d714-6c42-4091-91ee-40d368ab19d1.png)

Figure 5: LCNN race-wise accuracy

![Aspose Words 50618ed9-b1b2-4630-9df0-4f841fa4401b 006](https://user-images.githubusercontent.com/59523992/163758319-c0bff142-4a9e-4392-816f-e392b41d3d9b.png)

Figure 6: LCNN race-wise accuracy at focal loss

b) ROC curve for SVM and LCNN for gender prediction tasks. (Draw ROC curve from scratch.)
Results - ROC curve for SVM and LCNN for gender prediction tasks.

![Aspose Words 50618ed9-b1b2-4630-9df0-4f841fa4401b 007](https://user-images.githubusercontent.com/59523992/163758485-bd033a2e-6eee-42cb-90d8-d82221b82b35.png)

Figure 7: SVM ROC curve

![Aspose Words 50618ed9-b1b2-4630-9df0-4f841fa4401b 008](https://user-images.githubusercontent.com/59523992/163758544-b08708f3-2fd6-48c5-a43d-2ca40500365b.png)


Figure 8: LCNN ROC curve at cross-entropy loss

![Aspose Words 50618ed9-b1b2-4630-9df0-4f841fa4401b 009](https://user-images.githubusercontent.com/59523992/163758560-b7b08251-eaa0-4ac7-b12c-982a5fbb9a87.png)


Figure 9: LCNN ROC curve at focal loss

![Aspose Words 50618ed9-b1b2-4630-9df0-4f841fa4401b 010](https://user-images.githubusercontent.com/59523992/163758571-5d101353-4623-49e0-afeb-f7d7bd60f5c2.png)

c) Draw the Precision-Recall curve. (Draw Precision-Recall curve from scratch.)

Results - 

![Aspose Words 50618ed9-b1b2-4630-9df0-4f841fa4401b 011](https://user-images.githubusercontent.com/59523992/163758595-ab54a843-dfba-4229-b89b-9ea52b65260a.png)

Figure 10: SVM Precision curve

![Aspose Words 50618ed9-b1b2-4630-9df0-4f841fa4401b 012](https://user-images.githubusercontent.com/59523992/163758706-c1371211-c414-400c-a77c-ca734fd86e64.png)


Figure 11: LCNN Precision curve at cross-entropy loss

![Aspose Words 50618ed9-b1b2-4630-9df0-4f841fa4401b 013](https://user-images.githubusercontent.com/59523992/163758718-563c17f6-9ef5-4169-b754-a7b9070a5bcd.png)


Figure 12: LCNN Precision curve at focal loss

4. Of the two curves stated above, which is more reliable for biased/imbalanced
data? Why? Draw inferences from the observed results on why one ap-
proach (SVM or LCNN) performs worse/better than the other.
(a) ROC Curves summarize the trade-off between the true positive rate
and false positive rate for a predictive model using different proba-
bility thresholds.
(b) Precision-Recall curves summarize the trade-off between the true pos-
itive rate and the positive predictive value for a predictive model
using different probability thresholds.
(c) ROC curves are appropriate when the observations are balanced be-
tween each class, whereas precision-recall curves are appropriate for
imbalanced datasets.
4. Draw the Precision-Recall curve. (Draw Precision-Recall curve from scratch.)
5. Of the two curves stated above, which is more reliable for biased/imbalanced data? Why? Draw
inferences from the observed results on why one approach (SVM or LCNN) performs worse/better than
the other.
5. Do You observe any bias in the data ? Analyze the results.
6. Change the loss function to focal loss for LCNN. Now compare the results with previous loss function
that you have used ?

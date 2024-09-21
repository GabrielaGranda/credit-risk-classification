# Credit-Risk-Classification

**<h2>Analysis of the Classification Report:</h2>**

![image](https://github.com/user-attachments/assets/c733ffa5-dee6-40dd-b751-e3c6ead574d5)

**Healthy Loan (Majority Class):**
The model performs flawlessly when predicting Healthy Loans, with a precision, recall, and F1-score of 1.00 across the board. This means the model perfectly identifies all healthy loans without any false positives or false negatives. With a support of 18,759 instances, this strong performance is achieved on a large number of cases, indicating robust reliability for this class.

**High-Risk Loan (Minority Class):**
For High-Risk Loans, the model demonstrates good but not perfect performance. The precision is 0.87, meaning 87% of the loans predicted as high-risk were indeed high-risk. The recall is 0.89, indicating that 89% of all actual high-risk loans were correctly identified by the model. The F1-score, which balances precision and recall, is 0.88, showing a strong but slightly less perfect performance compared to Healthy Loans. This is based on a smaller support of 625 cases, which reflects the typical class imbalance between high-risk and healthy loans.

**Overall Accuracy:**
The model achieves an overall accuracy of 0.99, meaning it correctly classifies 99% of all loans, both healthy and high-risk, in the dataset of 19,384 instances. This high accuracy indicates that the model is highly effective overall.

**Macro Average:**
The macro average for precision, recall, and F1-score is 0.94, which is the unweighted mean of these metrics for both classes. This result reflects that while the model does exceptionally well for both healthy and high-risk loans, the slight drop in performance for high-risk loans lowers the average.

**Weighted Average:**
The weighted average for precision, recall, and F1-score is 0.99, showing that the overall performance is dominated by the more frequent healthy loans. Since this average accounts for the class imbalance, it reinforces the model’s strong performance, even though it slightly struggles with the minority class.

**Class Imbalance:**
The model’s performance is clearly influenced by the class imbalance, where Healthy Loans dominate the dataset. While this leads to excellent accuracy and precision for the majority class, it slightly compromises the detection of High-Risk Loans, evident from the lower precision and recall for this minority class.

**Key Insights:**
The model performs with near-perfect accuracy for Healthy Loans and does well for High-Risk Loans, but there is a small drop in precision (0.87) and recall (0.89) for high-risk loans. This suggests the model occasionally misclassifies some high-risk loans as healthy.
The overall accuracy of 99% is excellent, but the model could potentially benefit from strategies to handle the class imbalance better, such as further fine-tuning or using specialized methods like cost-sensitive learning.
The macro average of 0.94 reflects that the model’s performance is slightly less balanced between the two classes, while the weighted average of 0.99 shows the model excels primarily due to its strong performance on the more frequent healthy loan class.

**<h2>Metrics Derived:</h2>**

**Precision (Healthy Loans):** The precision for healthy loans is 1.00, meaning the model perfectly identifies all healthy loans without false positives.

**Precision (High-Risk Loans):** The precision for high-risk loans is 87.47%, meaning that 87.47% of the loans classified as high-risk are indeed high-risk, while 12.53% are false positives.

**Recall (Healthy Loans):** The recall for healthy loans is 1.00, indicating that the model correctly identifies 100% of healthy loans, without missing any true positives.

**Recall (High-Risk Loans):** The recall for high-risk loans is 89.28%, meaning that 89.28% of actual high-risk loans are correctly identified, while 10.72% are misclassified as healthy loans (false negatives).

**F1-Score for High-Risk Loans:** The F1-score for high-risk loans, balancing precision and recall, is 88.36%. This reflects the model’s capability to handle the minority class (high-risk loans), though it still misclassifies some as healthy.

**<h2>Confusion Matrix:</h2>**

![image](https://github.com/user-attachments/assets/e5db21c4-2971-45c8-9eba-74b8eab7eaad)

**True Positives (Healthy Loans):** 18,679 correctly classified as healthy.

**False Positives:** 80 healthy loans misclassified as high-risk.

**False Negatives:** 67 high-risk loans misclassified as healthy.

**True Negatives (High-Risk Loans):** 558 correctly classified as high-risk.

**<h2>Conclusion:</h2>**
The model exhibits excellent performance overall with an accuracy of 99.24%, particularly excelling in predicting healthy loans. However, while it performs well on high-risk loans (with a precision of 87.47% and recall of 89.28%), the class imbalance affects its ability to perfectly predict high-risk loans. Further refinement, such as balancing techniques (e.g., oversampling, undersampling), could enhance the model’s performance for the minority class.






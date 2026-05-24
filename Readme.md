## Defect Detection in Hot Rolling Mills (Max. Score: 100)## Project Overview
The "Alpha Defect" is a critical quality challenge in hot rolling mills. It cannot be detected inline because the steel coil remains under tension in the inspection zones.
Current quality control relies on destructive or manual sample observations at the final stage, checking only a small percentage of total coils. Manual inspection is highly time-intensive, creating a bottleneck for strict manufacturing and supply chain timelines. While the alpha defect accounts for a small percentage of production, it causes customer complaints and costly product downgrades. [1, 2, 3, 4, 5] 
## Objective
Predict the occurrence of the alpha defect during the rolling process using multi-stage process parameters ($X1$ to $X49$) to enable proactive quality control and eliminate customer complaints.
------------------------------
## Dataset Description
The dataset contains multi-stage process parameters captured during production.
## File Dimensions

* train.csv: 1352 rows × 51 columns
* test.csv: 339 rows × 50 columns
* sample_submission.csv: 339 rows × 2 columns

## Variable Description

| Column Name | Description |
|---|---|
| coilid | Unique identifier for each manufactured steel coil |
| x1 to x49 | Process parameters measured across multiple manufacturing stages |
| y | Target variable: Alpha defect occurrence (1 = Defect, 0 = No Defect) |

------------------------------
## Evaluation Metric
Submissions are evaluated automatically based on strict confusion matrix thresholds to ensure zero defective coils reach the customer.

* Recall: 100% (Exactly 0 False Negatives allowed)
* Precision: > 90% (Less than 10% False Positives allowed)

------------------------------
## Submission Criteria
Your final output must strictly follow these constraints to avoid automated rejection:

* Format: .csv file format only
* Dimensions: Exactly 339 rows × 2 columns
* Required Columns:
1. coilid: Must match the exact identifiers in test.csv
   2. y: Predicted binary classification (0 or 1)

------------------------------
## Getting Started## 
Given the strict 100% Recall requirement, standard probability thresholds (0.5) will likely fail.

   1. Handle Imbalance: The alpha defect is rare; use class-weighting or SMOTE.
   2. Optimize Thresholds: Lower the classification threshold during prediction to eliminate False Negatives.
   3. Metric Focus: Tune hyper-parameters using recall as the primary scoring metric, while monitoring precision.

------------------------------

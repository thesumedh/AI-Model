Defect Detection in Hot Rolling
Max. score: 100
In Hot Rolling Mills, one specific defect (referred to here as the Alpha defect) is a critical quality challenge. This defect cannot be detected through the existing system because the coil remains under tension in the inspection zones. Since it is not possible to detect Alpha defects inline, current quality control relies on sample observations at the final stage, where only a certain percentage of the total coils produced are inspected. Additionally, manual inspection is time-intensive, whereas the manufacturing and supply chain processes operate under strict time constraints. Although the Alpha defect accounts for only a very small percentage of the total production volume, it can still lead to customer complaints and product downgrades.
 
Task
During hot rolling, each stage has different process parameters that can contribute to the formation of the defect. Therefore, all stages must be considered to effectively detect the formation of Alpha defects.

Detect the occurrence of the Alpha defect during rolling to prevent customer complaints and reduce downgrades through proactive action.

Dataset Description

The dataset folder contains the following files:

File	Dimensions
train.csv	1352 × 51
test.csv	339 × 50
sample_submission.csv	339 × 2
Variable Description

Column Name	Description
CoilID	Unique identifier for each coil
X1–X49	Process parameters across multiple stages
Y	Target variable: Alpha defect occurrence (1 = Defect, 0 = No Defect)
Evaluation Metric

A model which will have 0 false negative and less than 10% False positive will be accepted.

Recall – 100%
Precision - > 90%
Submission Criteria

The submission file must be submitted in .csv format only.
The size of this submission file must be 339 × 2.
Ensure that your submission file contains:
Correct CoilID values as per the test file
Correct column names as provided in the sample_submission.csv file
Instructions

Click Download dataset to download the dataset.
Solve the problem in your local environment.
Save the predictions in a .csv file named expected_submission.csv.
Click Upload File (under the Upload File section) to upload your prediction file (.csv).
Click Upload File (under the Upload Source Code section) to upload your .ipynb file along with any presentation file.
Add any instructions or comments in the Your Answer section.
Click Submit.

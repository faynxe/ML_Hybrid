## Credit risk prediction and explainability and bias detection with Amazon SageMaker

In this workshop, we demonstrate a end to end ML use case of credit risk prediction with model explainability and bias detection. We use a well known open source dataset https://archive.ics.uci.edu/ml/datasets/South+German+Credit+%28UPDATE%29 .
We show how to use SageMaker Clarify to run bias detection on a SageMaker inference pipeline model. We include the bias reports from Clarify as well as relevant links to further resources on this subject.

The notebook performs the following steps:

1. Upload, train, and captured inference dataset to s3.
2. Create a SageMaker Inference pipeline containing the SKlearn and XGBoost model in a series
3. Run SageMaker Clarify Bias on train dataset to get baseline bias metrics.
4. Run SageMaker Clarify Bias job on captured dataset (inference data plus merged groundtruth label) to get bias metris.
5. Compare the bias metrics from the capture data to the baseline bias metrics within a contraint threshold.
6. Create a dataframe to show if any metrics exceeded the constraints









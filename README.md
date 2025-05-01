# master_thesis_Christina_Petschnig


Repository Structure
1) dataset_manually_annotated

Contains the manually annotated articles, which serve as the ground truth for evaluation.

The output/ subfolder includes the extracted entities from these articles.

2) gliner

fine-tuning/:

Includes synthetically generated datasets for fine-tuning.

Contains the fine-tuned models.

Stores loss curves.

Includes the Jupyter Notebook used for fine-tuning on Google Colab with different configurations.

dataset/:

Contains tokenized articles prepared for Gliner, due to its token length limit.

tests/:

quality_tests/:

Contains tests for label refinement

Each test includes two files:

Files starting with gliner... are used to send labels to the model and process predictions.

Files starting with matching... calculate evaluation metrics such as precision, recall, and F1 score.

The output/ subfolder contains plots of the test results.

quantity_tests/:

Tests with using the final label set on the different models (+ also the base label set on Gliner Large News v2.1).

The specific model used is indicated in the file names.

The output/ subfolder contains plots visualizing these outcomes.

3) gpt-4o-mini

Contains the calculation of evaluation metrics using the GPT-4o-mini model.

4) efficiency_tests

Includes calculations for testing model efficiency

5) comparison

Contains comparisons of the different models 

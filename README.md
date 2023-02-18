# CommonLit Readability Prize

CommonLit, Inc., is a nonprofit education technology organization serving over 20 million teachers and students with free digital reading and writing lessons for grades 3-12.
With Georgia State University, an R1 public research university launched this <a href="https://www.kaggle.com/competitions/commonlitreadabilityprize/overview">Kaggle competition</a> on May 3, 2021 to improve redability rating methods.

We will be predicting the reading ease of excerpts from literature.

# Dataset

## Files
- train.csv - the training set
- test.csv - the test set
- sample_submission.csv - a sample submission file in the correct format
## Columns
- id - unique ID for excerpt
- url_legal - URL of source - this is blank in the test set.
- license - license of source material - this is blank in the test set.
- excerpt - text to predict reading ease of
- target - reading ease
- standard_error - measure of spread of scores among multiple raters for each excerpt. Not included for test data.

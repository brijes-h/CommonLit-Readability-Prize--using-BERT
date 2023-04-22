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

# BERT 

In this project, BERT model is used to  predict the readability of text samples BERT (Bidirectional Encoder Representations from Transformers) is a state-of-the-art language model developed by Google. It is a deep learning model that is able to capture the context of words in a sentence in both forward and backward directions. This allows the model to understand the relationships between words in a sentence and produce highly accurate predictions.
<br>

![image](https://user-images.githubusercontent.com/91772980/233765519-7ad5be1e-5f4b-4836-82f4-f5c7a2eee5eb.png)
<br>
<br>
In this project, we use BER-Base-Uncased to fine-tune on the CommonLit Readability Prize dataset. BERT Base Uncased is a pre-trained BERT model that was trained on lower-cased English text. It has: 
<br>


| Model | Layers | Hidden Units | Parameters |
|-------|--------|--------------|------------|
| BERT Base Uncased | 12 | 768 | 110 million |

The "uncased" part of the name means that the model was trained on text that was converted to lower case. This means that the model treats "hello" and "Hello" as the same word, and reduces the size of the vocabulary.


## Accuracy Metric

The accuracy metric used in this project is Mean Squared Error (MSE). The MSE is a measure of how well a regression model is able to predict the outcome variable. It is calculated by taking the average of the squared differences between the predicted values and the actual values. A lower MSE indicates better performance of the model.

## Loss Functions

The loss function is a measure of how well the model is able to predict the outcome variable during the training process. In this project, the loss function used is Mean Squared Error (MSE) as well. During training, the model is optimized to minimize the MSE loss.

## Output
<table>
  <tr>
    <td><img src="loss.png" alt="Image 1"></td>
    <td><img src="mse.png" alt="Image 2"></td>
  </tr>
</table>


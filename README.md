# CA4023 - Natural Language Technologies : Assignment 2

## Assignment Structure

This assignment contains two tasks:

1. <b><u>Part One:</u> Improve the Accuracy of Logistic Regression in 2 Different Ways</b>
    * Given the accuracy of a logistic regression model trained on an IMDB database of movie reviews, consider two ways that the model can be adjusted to improve the accuracy.
    * The accuracy, which stands at 77%, was achieved using an 80/20 split of the 25,000 rows of training data.

2. <b><u>Part Two:</u> Analyse/Improve/Fine-Tune BERT</b>
    * This section of the assignment allows you to choose an area of BERT to work on.
    * The first option is to perform an analyses of BERT.
        * This option requires you to compare the performance of BERT to the performance of the logistic regression model in Part One. 
        * You can investigate the strengths and weaknesses of the model and explore examples that could 'break' each model.
    * The second option is to improve BERT's Text Selection Process.
        * BERT has a limit of 512 tokens as input. If input is longer than 512 tokens, the first 512 tokens are accepted as input.
        * This option requires you to investigate new ways to select the sections of the review that should be included in the input to the BERT model.
    * The third option is to fine-tune BERT on a new dataset/task.
        * BERT was initially trained for masked token prediction and predicting whether to sentences follow each other.
        * BERT has since been fine-tuned to perform various NLP tasks. 
        * This option requires you to fine-tune BERT to perform a different NLP task.

## Repository Structure

There are two directories in this repository, one for each task. These directories are structured as follows:

1. <b><u>Part_1</u></b>
    * [First Attempt at Improving Accuracy.ipynb](Part_1/First\ Attempt\ at\ Improving\ Accuracy.ipynb): This is a notebook that contains the first attempt at improving the Logistic Regression Accuracy. This notebook explores the effect of changing training/testing splits.
    * [Second Attempt at Improving Accuracy.ipynb](Part_1/Second\ Attempt\ at\ Improving\ Accuracy.ipynb): This notebook contains the second attempt at improving the Logistic Regression Accuracy. This notebook explores the functionality of the CountVectorizer() function, by removing stop words, using a custom re-distributed input vocabulary and applying stemming to the reviews.

2. <b><u>Part_2</u></b>
    * [data](Part_2/data): This is a directory that contains three CSV files. These files are the original (cleaned) CrowS-Pairs dataset, and the two restructured versions of this file (one for training, one for testing).
    * [Adjusting CrowS-Pairs Dataset.ipynb](Part_2/Adjusting\ CrowS-Pairs\ Dataset.ipynb): This is a notebook that goes through the process of re-structuring the data in order to make it usable for the BERT model.
    * [Fine_Tuning_BERT_on_Stereotyped_data.ipynb](Part_2/Fine_Tuning_BERT_on_Stereotyped_data.ipynb): This is a notebook that trains and evaluates BERT when it has been fine-tuned as a multiclass classifier model for identifying stereotype, antistereotype and non-stereotype sentences.
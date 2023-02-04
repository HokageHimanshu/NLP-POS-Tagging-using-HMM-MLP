# :pushpin: NLP: HMM and MLP Classifier

Part-of-Speech Tagging is implemented using HMM and MLP models.

* **Task 1** - Design and implement Hidden Markov Model (HMM) based Part-of-Speech (POS) tagger implementing Viterbi algorithm with the following assumptions. Markov assumption length 1 - Probability of any state sk depends on its previous state only, i.e., P(sk| sk-1 ) <br>

* **Task 2** - Design and implement a MLP-based Part-of-Speech (POS) tagger implementing the following.<br>
	1. Create Word2Vec & Glove representations of each word. Compare their performances.<br>
	2. Use the representation of each to perform the task of POS tagging using multi-layer perceptrons(MLP).

Perform 3-fold cross validation on the dataset performing both Task 1 and 2 and show a comparative study (tabular) on following basis: <br>
* Precision, recall and F1-score.
* Tag-wise precision, recall and F1-score
* Confusion matrix (Each element Aij of matrix A denotes the number of times tag i classified as tag j).
* Statistics of tag set.


glove and word2vec embedddings can be downloaded from [here](https://drive.google.com/drive/folders/1eMU1eRJTHUg4N8vIAZJ610_-ve0F0fu8?usp=sharing).

Note - 
* Some cells have the starting comment as optional which means that they can be skipped.
* Word2vec model has been trained. Pretrained model was not working on the current system specs.


## :technologist: Requirements

:package: sklearn <br>
:package: gensim <br>
:package: numpy <br>
:package: pandas <br>

## :card_file_box: Files
* 'Report.pdf': Contains the complete report for the exercise.<br>
* 'code.ipynb' : Contains the code for the exercise.<br>
* 'Brown_tagged_train.txt' : Dataset for the exercise. Sentences are already tokenized. Cases where word itself contains / is considered as a single word like a/b. <br>
* MLP*FOLD or HMM*FOLD folders - contains fold wise statistics like tag stats, confusion matrix
* HMM_incorrect_classifications or MLP_incorrect_classifications  - examples that are incorrectly classified

## :monocle_face: Results

| |HMM |MLP|
|---|----|-----|
|Precision|0.86|0.86|
|Recall|0.84|0.82|
|F1 score|0.84|0.82|
|Accuracy|0.91|0.90|	



Check out Report.pdf for complete results.

## Acknowledgments
This exercise was a part of NLP course.

:star: Have you found this repository helpful? Give it a star to show your support! :star:


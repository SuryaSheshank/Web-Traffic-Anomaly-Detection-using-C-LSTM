# Web-Traffic-Anomaly-Detection-using-C-LSTM
  * This repository contains code to implement the research paper which closely simulate those run by Tae-Young kim,Sung-Bae Cho. The research paper can be found [here.]  (http://sclab.yonsei.ac.kr/publications/Papers/IJ/2018_ESWA_TYK.pdf)
  * This Yahoo S5 dataset has been borrowed from this link https://github.com/harris0704/nbaData16-17/tree/master/Yahoo_S5_Data

The model was tested on test data(Which is 30% of total data). The final test results for training the model for 500 epochs(as mentioned in the paper) are:

* Accuracy -  94.6%
* Precision - 68.4%
* Recall -    73.03%
* F1-Score -  70.06%

# Conclusions from the experiment

* The Accuracy and F1-Score of the model increases as we increased the training epochs to 500.

* Changing loss function from mean-square-error to binary-cross-entropy also increased performance of the model because, this is a classification problem binary-cross-entropy loss   function gives more accurate results.

* Combining CNN with LSTM greatly helped in detecting patterns and classifying anamolies with good accuracy and precision than most of LSTM networks.

# Instructions to run

Paste the link https://github.com/SuryaSheshank/Web-Traffic-Anomaly-Detection-using-C-LSTM in Google Collab as a GitHub repository
Open up 'CLSTM.ipynb' 

You can keep track of training the model through 'accuracy' metrics and if you dont want that just comment the 'Metrics' in model.fit() method.

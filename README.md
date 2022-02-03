# SignLanguageInterpreter
Using a combination of Recurrent Convolutional Neural Network and LSTM to accurately recognize a complete _word_ formed using sign-language (hand images) characters. 

You simply have to execute the main notebook named as Master_notebook_group10.ipynb

Training requires big dataset which can be downloaded here https://www.dropbox.com/s/xgbb96to10aggrn/dataset.rar?dl=0

In order the run the master notebook, following auxilliary files are required:

1. global_defs.py: This file contains the 'device' declaration. Ig running on CUDA enabled device, please comment-out the 'cpu' forcing part.

2. CNN_Utils.py: contains some utility functions, such as data loading, training, testing etc. for the Training of baseline CNN.

3. seq2seq_utils.py: contains some utility functions, such as data loading, training, testing etc. for the Training of Sequence-to-Sequence model.

4. DataGen_Utils.py: contains utility functions for Data Pre-processing and Augmentation

5. Analysis_Utils.py: contains utility functions for final evaluation and comparison of all models.

All these auxilliary modules are imported into master notebook. 


In addition to the main report part in the master notebook, we have also added code to run the training' notebooks at the end of the master notebook for various models.


Currently, it recognizes only single gesture characters (e.g. 'A', 'B', 'C', etc.). However, actual sign language usually works at the word level, i.e. gestures are words, not characters. Recognizing word gestures is the next planned step.

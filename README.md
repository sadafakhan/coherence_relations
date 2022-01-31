## Description

This program performs coherence relation sense classification. It reads in Glove embedding vectors from an input text file, loads in training and test coherence relation classification data from a subset of CoNLL resource files, and creates training and test vectors from this data. 

It then outputs a .csv formatted file of the training and test instances, and trains a scikit-learn classifier on the training instances. It then implements the classifier on the test instances and writes to an output file: 

* the overall per-class F-measure
* For each test instance: "[true_label]   [predicted_label]"
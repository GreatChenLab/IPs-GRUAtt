# IPs-GRUAtt
**An Attention Mechanism-Based Bidirectional Gated Recurrent Unit Network for Predicting Phosphorylation Sites of SARS-CoV-2 Infection**

![image](https://user-images.githubusercontent.com/90399926/217559241-2e3fc19c-5cf2-435d-ba6d-91420263c151.png)

The deep learning model framework based on Bi-GRU and attention mechanism to predict the phosphorylation sites of SARS-CoV-2 infection. Given a protein sequence, it is encoded by an embedding layer and then fed into the Bi-GRU structure. After Bi-GRU, we add dropout to prevent model overfitting, and also use an attention mechanism layer to capture the position information of the protein sequence. Finally, the input protein sequences are discriminated by a fully connected layer. The experimental results show that IPs-GRUAtt surpassed the existing methods for identifying phosphorylation sites.

## Must installed packages or softwares

- Pandas==0.23.4

- Numpy==1.19.0

- Tensorflow==2.0.0

- Skikit-learn==1.0.2

## Webserver
[http://cbcb.cdutcm.edu.cn/phosphory/](http://cbcb.cdutcm.edu.cn/phosphory/)

## Coda
1. train.ipynb is the model training for S/T phosphorylation sites and Y phosphorylation sites;
2. test.ipynb is the prediction of S/T phosphorylation sites and Y phosphorylation sites.

## Data
1. The file "data" contains all the data used in this study. st-train.fa and st-test.fa are the training set and test set of S/T phosphorylation sites, respectively. y-train.fa and y-test.fa are the training set and test set of Y phosphorylation sites.

## Model
1. The file "model" contains the final model weights for the independent tests. t_model.h5 is the final model weight for S/T phosphorylation sites; y_model.h5 is the final model weight for Y phosphorylation sites.

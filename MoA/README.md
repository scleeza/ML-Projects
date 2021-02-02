# Mechanisms of Action (MoA) Prediction

- [Data Description](https://www.kaggle.com/c/lish-moa)

- [Notebook link](https://www.kaggle.com/scleeza/cv6-tfa-labeling)


## Quick View
__Goal__: Predict MoA (only 0 and 1) from data of gene and cell vitality, build multiple binary classifier

__Metrics__: minimum Log loss

__Procedure__:

 - Imbalance Data:
    - MoA tag are extremely imbalanced, average 89 positive tags in each column from 21K entries
        ```python
          
        ```
    - Label Smoothing has been conducted to help improve accuracy in this multiple output case[A great explanation here](https://www.pyimagesearch.com/2019/12/30/label-smoothing-with-keras-tensorflow-and-deep-learning/)
    
    - Simple Data Merge on Cell and Gene data
    
    - Use Pipeline function to automatically finished
        - Numerical data
         - Quantile transform
         - PCA
        - Categorical
         - One-hot-labeling  
         
    - Build DNN model with 3 NN layer     
    - Use __keras.tuner__ to do hyper parameters tuning [Notebook](hyperparam.ipynb)
    
    



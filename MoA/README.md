# Mechanisms of Action (MoA) Prediction

_Data Source : [Data Description] (https://www.kaggle.com/c/lish-moa)

_Public Notebook: [kaggle](https://www.kaggle.com/scleeza/cv6-tfa-labeling)


## Quick View
__Goal__: Developed a DNN model to classify whether a 

__Metrics__: None, this was unsupervised learning goal.

__Results__:

- Kmodes is a clustering method focus on categorical data.
- Some columns contain too many values, so appropriate clean techniques were applied to simplified data into categorical type.
- The estimation is conducted by comparing cost value between variant number of clusters, the optimal point should see decreasing rate of cost started to slow.
- The results shows that 5 clusters is optimal.
- To maintain certain diversity, I give a small probability to let small group (e.g. ppl in Art or business major) be able to join with major group(e.g. ppl in CS major).
- Of course cosine similarity is a solution to this.
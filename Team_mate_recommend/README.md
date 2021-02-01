# Find teammates using K-Mode clustering.
_Data Source : 2020 TAMU Datathon Competition_
_sklearn, pandas , numpy, seaborn_

## Quick View
__Goal__: Develope a way to recommend team mates for future event, data based on applicants' questionarie answer. (e.g. School, location, major...etc)

__Metrics__: None, this was unsupervised learning goal.

__Results__:

- Kmodes is a clustering method focus on categorical data.
- Some columns contain too many values, so appropriate clean techniques were applied to simplified data into categorical type.
- The estimation is conducted by comparing cost value between variant number of clusters, the optimal point should see decreasing rate of cost started to slow.
- The results shows that 5 clusters is optimal.
- To maintain certain diversity, I give a small probability to let small group (e.g. ppl in Art or business major) be able to join with major group(e.g. ppl in CS major).
- Of course cosine similarity is a solution to this.

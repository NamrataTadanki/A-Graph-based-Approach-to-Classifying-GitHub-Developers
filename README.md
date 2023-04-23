# A-Graph-based-Approach-to-Classifying-GitHub-Developers
The objective of our project is to perform node classification on a GitHub network to predict if a specific developer is a web developer or a machine learning developer.

## Dataset Description
We are using a dataset of GitHub’s large social network which was collected by public API in 2019 sourced from Snap Stanford. This dataset is undirected where nodes represent developers who starred in at least 10 repositories and a collection of edges represents the social network of GitHub users, where an edge between two users indicates that they are following each other on GitHub. The dataset also includes the attributes of each user, such as their number of followers, number of repositories, and programming language preferences. There are also vertex features associated with each node giving additional information about the developer. These features were extracted based on geographical location, specific repositories in which the developer was featured, the employer, and the developer’s e-mail address.
 - Number of nodes: 37700
 - Number of edges: 289003
 - Min. degree: 1
 - Max. degree: 9458
 - Mean degree: 15.331724137931035
 - Median degree: 6.0
 - Density: 0.0004066878203117068
 - The graph is directed:  False
 
 ## Feature Extraction
1. Graph Features
 - Degree Centrality
 - Eigenvector Centrality
 - PageRank
 - Clustering Coefficient
 - Betweennesses Centrality
2. Community Based Features
3. Principal Component Analysis 

## Algorithms 
1. NODE2VEC and DeepWalk 
2. Logistic Regression 
3. Random Forest
4. XGBoost
5. Graph Attention Network (GAT) 
6. Graph Convulational Network (GCN)

## Evaluation

For the node classification problem being solved with GCNNs, we used cross entropy as the loss function, and accuracy as the metric. To evaluate the performance of the other algorithms, we used standard metrics such as accuracy, precision, recall, and F1 score. Since our dataset is imbalanced, we also considered using metrics such as Area Under the Precision-Recall Curve (AUPRC) or Balanced Accuracy. 


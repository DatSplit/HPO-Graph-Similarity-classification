# HPO-Graph-Similarity-classification
Graph Similarity classification on HPO graphs of patients with a genetic disorder
![gex](https://user-images.githubusercontent.com/68016450/145811836-40dfe402-b4e4-457e-ab7b-edea3f2de729.png)

2 implemented frameworks for graph similarity classification on HPO graphs.

The first framework is the most common subgraph (MCS) framework which
 consists of the following 4 classification methods:
  * most common subgraph classification based on the amount of nodes in the MCS.
  * most common subgraph classification based on the amount of edges in the MCS.
  * most common subgraph classification based on the sum of edge weight in the MCS.
  * most common subgraph classification based on the amount of nodes in the MCS corrected by the size of the input graphs.
  

The second framework is the graph kernel classification framework which consists of the following classification method:
  * graph kernel classification in combination with the GraKeL package (https://ysig.github.io/GraKeL/0.1a8/) and support vector machines.
  

  
    4 parameters need to be provided to run this model:
    * The data
    * Choose one graph kernel from this list (VertexHistogram,WeisfeilerLehmanOptimalAssignment,ShortestPath,EdgeHistogram)
    * choose K
    * Choose KFold ('default') or stratified KFold ('stratified')
    
    ``` graph_kernel_classification(pd.read_pickle('C:/Users/niels/Downloads/patienten.pkl'),VertexHistogram,553,'kfolds')```
    
    
    
    

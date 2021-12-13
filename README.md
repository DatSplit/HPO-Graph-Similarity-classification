# HPO-Graph-Similarity-classification
Graph Similarity classification on HPO graphs of patients with a genetic disorder
<img title="a HPO graph" alt="" src="E:\big_downloads\gex">


2 Frameworks for graph similarity classification on HPO graphs are implemented in this repository.

The first framework is the most common subgraph (MCS) framework which consists of the following 4 classification methods:
  * most common subgraph classification based on the amount of nodes in the MCS.
  * most common subgraph classification based on the amount of edges in the MCS.
  * most common subgraph classification based on the sum of edge weight in the MCS.
  * most common subgraph classification based on the amount of nodes in the MCS and corrected by the size of the input graphs.
  


The second framework is the graph kernel classification framework which consists of the following classification method:
  * graph kernel classification
  
  
    4 parameters need to be chosen from when running the model:
    * Supply the data
    * Choose one graph kernel from this list (VertexHistogram,WeisfeilerLehmanOptimalAssignment,ShortestPath,EdgeHistogram)
    * choose K
    * Choose KFold or stratified KFold
    
    ```python graph_kernel_classification(pd.read_pickle('C:/Users/niels/Downloads/patienten.pkl'),VertexHistogram,553,'kfolds')```
    
    
    
    

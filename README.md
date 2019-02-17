NetworkHub: Prioritize hub gene node regulation with intra-network association
============
**Citation:** Hung-Ching Chang, Chiao-Pei Chu, Shu-Ju Lin, Chuhsing Kate Hsiao (2019) NetworkHub: Prioritize hub gene node regulation with intra-network association.

# Overview 
`NetworkHub`is a tool for identifying the influential hub genes in a gene-set or pathway. The method is described in detail in *Hung-Ching Chang, Chiao-Pei Chu, Shu-Ju Lin, Chuhsing Kate Hsiao (2019) NetworkHub: Prioritize hub gene node regulation with intra-network association.*


# Tutorials
* There are 7 functions, one R markdown document and two data in the example.
* Manual pages `Example_of_NetworkHub` are good places to start with. It demonstrates a complete test run with an example. [PDF file](https://github.com/Hung-Ching-Chang/NetworkHub/blob/master/Example_of_NetworkHub.pdf)
* `NetworkHub` is the major function. [link](https://github.com/Hung-Ching-Chang/NetworkHub/blob/master/Functions/NetworkHub.txt)

# Introduction to functions
* Pre-processing
  1. `KGML_to_Matrix` is responsible for transferring the KGML file to a directed adjacency matrix.
  2. `trans2undirected` is a function for transferring a directed adjacency matrix to an undirected adjacency matrix.
  3. `sub_expression_data` transforms the expression data from the gene level to the node level.
  4. `remove_missing_node` can remove nodes whose expression levels were not measured.
* Intra-network analysis
  1. The major function `NetworkHub` is a pathway analysis for gene expressions. 
  2. `rank_node` ranks the nodes inside the target pathway.
* Pathway test
  1. `pathway_permute` performs the pathway association test with the p-value calculated by permutation.

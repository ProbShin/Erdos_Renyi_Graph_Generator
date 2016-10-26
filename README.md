# Erdos-Renyi-Graph-Generator
a matlab version of Erdős Rényi Random Graph generator.

### [Erdős–Rényi model](https://en.wikipedia.org/wiki/Erd%C5%91s%E2%80%93R%C3%A9nyi_model)

The orignal two definiations are:

* In the *G(n,M)* model, a graph is chosen uniformly at random from the collection of all graphs which have *n* nodes and *M* edges. 
* In the *G(n,p)* model, a graph is constructed by connecting nodes randomly.

*we used the second one, since the first one can be easily transformed into the second one by `p=2M/(n(n-1))`*  

### Important Notes
This code only generate approximately Erdos-Renyi Random Graph. 
Since Erdos-Renyi Model only consider the undirected, non-self-loop
graphs. However, this code would firstly create a directed graph with,
self-loops. And then transform the directed graph into undirected simply
by ignore the upper triangular adjacency matrix and delete the self-loops  
        
However, when the graph size *n* is large enough, the generated graph would
approximately similar to the expected Erdos-Renyi Model.


### Description:
this function create Erdos-Renyi random Graph

### Date: 
Oct 25 2016

### Output Arguments:
     G : generated random graph
     n : graph size, number of vertexes, |V|
     m : graph size, number of edges, |E|

### Input Arguments:
*        n : graph size, number of vertexes, |V|
*        p : the probability p of the second definition of Erdos-Renyi model.
*        seed: seed of the function. 
*        format:
*        opt:

### Thanks to the contributors: 
X.C.
*contribute to append your name here*

### LICENSE:
[BSD-2-Clause](https://opensource.org/licenses/BSD-2-Clause)



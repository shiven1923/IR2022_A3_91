# IR2022_A3_91
Link Analysis, PageRank, Hubs and Authorities  
  
The Network is taken from Wiki-Vote.txt from : https://snap.stanford.edu/data/wiki-Vote.html  

Link Analysis  
1. Number of Nodes = 7115
2. Number of Edges = 103689
3. Average In-Degree = 14.573295853829936  
Formula Used = Sum(In-Degree of all Nodes)/(Number of Nodes)
4. Average Out-Degree = 14.573295853829936  
Formula Used = Sum(Out-Degree of all Nodes)/(Number of Nodes)
5. Node having Maximum In Degree = Node ID 4037
6. Node having Maximum Out Degree = Node ID 2565
7. Network Density = 0.0020485375110809584  
Formula Used = (Number of Edges)/(7115 x 7114)

(IN/OUT) Degree Distribution in the Q.ipynb file  
X-Axis : (IN/OUT) Degree  
Y-Axis : (Frequency of (IN/OUT) Degree)/(Number of Nodes)  

Local Clustering Coefficient in the Q.ipynb file  
Formula Used:  
LCC(node i) = (Number of edges in Ni) / (ni * (ni-1))  
where,  
Ni are the neighbouring nodes of node i  
ni is the number of neighbouring nodes of node i  


PageRank, HITS Hubs and Authorities  
Since PageRank algorithm ranks the nodes on the basis of incoming links to a node, we see 4037 node being given the highest rank.  
4037 is the node having maximum in-degree.
HITS Authorities also computes rank on the basis of incoming links (or hubs) and we see 4037 node at 2nd highest rank.  
Out of the top 20 nodes by PageRank and by HITS Authority, 9 are common indicating both algorithms using similar type of information for ranking.  
However out of the top 20 nodes by PageRank and by HITS Hub, only 1 is common since hub score is based on outgoing links unlike in PageRank.
The top 3 authorities are 2398,4037,3352 and top 3 hubs are 2565,766,2688. The top hub 2565 is also the node having maximum out degree  
again indicating that top hubs are based on the number of outgoing links. 2565 hub has outgoing link to all the top 3 authorities.


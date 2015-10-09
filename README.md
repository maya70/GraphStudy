# GraphStudy
The file randadj.py contains script to generate a random graph
Command line arguments: Number of nodes , number of edges (exact values) for the generated graph
The script generates a random adjacency matrix with the size specified, then adjusts the number of edges to the exact value provided by the user. 
Edge adjustment is a performance bottleneck in larger size of graphs (about 1 minute runtile for 1000 nodes with 1000 edges)
The script then generates random string labels for each one of the nodes that have at least one edge connection (non connected nodes are discarded here)
Next, the script writes a sql table with edges between nodes acting as primary key (also there is a column for edge weights that is currently set to 1.0 as a default value)

TODO1: verify file writes are performed correctly 
TODO2: add a function to create a series of such graphs according to a user-entered change factor 

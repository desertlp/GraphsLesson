# Graphs

## About graphs (Lora):
A graph is a collection of nodes, which store data, and edges. Edges represent relationships or connections between nodes.
Graphs are a powerful and flexible data structure, and have been widely adopted in modern software engineering.

Graphs are represented one of two ways in code: an adjacency list, or an adjacency matrix. Adjacency lists use a collection of arrays, where each node has its own array that lists the connected nodes. Adjacency Matrices are represented by a two-dimensional array, where 1 represents a connection (edge) and 0 represents a lack of an edge. 

## Examples of graphs (Zach):

#### Google Maps
Here, vertices are where roads meet, and edges are the roads themselves. Thus their navigation can find the shortest path between two vertices using weights (for distance, traffic, speed limit, etc). Given that not all roads are two-way, this will be a Weighted, Directed graph.

#### Instagram
Here, vertices are not only users, but their images, their likes, and their comments. Edges are the connections between these (A user makes a comment on another user’s photo). Since users may follow each other (but not necessarily be followed back), this is an Unweighted, Directed graph.

#### Facebook 
Facebook ‘friends’ are a great example of undirected graph, any of your friends are also friends with you. This is unlike Instagram followers who you may choose to follow, but they may follow you regardless.

#### Wikipedia
Like most of the internet, the web pages here are the vertices, and the links to pages are the edges. This is another example of a Directed graph (links only go one way), and was the basic idea behind Google’s initial Page Ranking Algorithm.

## What can be solved with graphs? (Will) 

Finding the shortest path between two nodes (breadth first). 

Weighted edges help us determine the path of least *cost* to the client.
‘Cost’ could be distance (for maps), expense (for programming), or resource allocation (for OSs)

Save on time by stashing common connections to prompt easier load times.

## Common Interview Questions (Leah & Timothy)

### The most common questions interviewers may ask you about graph data structures :

#### What is a connection between two nodes called?  

A connection between two nodes is called an edge. An edge is represented as a line (undirected edge) or an arrow (directed edge).

* Undirected edges represent bidirectional connections, like a friendship on facebook.

* Directed edges represent an unidirectional connection, like a follow on instagram. For example, you may follow an account, but it will not necessarily follow you back.

![Image of Directed vs Undirected Graphs](https://www.e-education.psu.edu/geog597i_02/sites/www.e-education.psu.edu.geog597i_02/files/Lesson8/Geog597i_Lesson8_directedgraph.jpg)


#### What is the difference between a tree and a graph?

Trees are a subset of graph wherein all nodes are connected upward to a parent node. Graphs have no requirements on how connections (edges) work.
    Both Breadth-First and Depth-First searches may be utilized on graphs, but be sure to use a ‘visited’ boolean as Graphs may contain cycles (trees will not).

![Image of Tree vs Graph](https://miro.medium.com/max/700/1*rguQ2Y2Z920IYGkO0cHHtQ.jpeg)


#### What do adjacency lists and matrices look like?

        Adjacency list:
            let graph = {
            'A': ['B', 'E'],
            'B': ['A', 'C', 'D', 'E'],
            'C': ['B', 'D'],
            'D': ['B', 'C', 'E'],
            'E': ['A', 'B', 'D'],
            }

Adjacency Matrix:

![Adjacency Matrix](https://cdncontribute.geeksforgeeks.org/wp-content/uploads/adjacencymatrix.png)


## Additional Resources

Some graph data structure [interview question topics.](https://medium.com/@codingfreak/graph-data-structure-interview-questions-and-practice-problems-22d5cd488855)

Visualizations of [breadth-first search](https://www.cs.usfca.edu/~galles/visualization/BFS.html) and [depth-first search](https://www.cs.usfca.edu/~galles/visualization/DFS.html) in a graph structure.

[Common interview questions](https://stackabuse.com/graph-data-structure-interview-questions) about graphs that don’t necessarily deal with coding.

[All about Dijkstra path-finding in graphs.](https://medium.com/basecs/finding-the-shortest-path-with-a-little-help-from-dijkstra-613149fbdc8e)

Practice [building a graph visually.](https://visualgo.net/en/graphds)

How Facebook shifted [from text input fields to a graph](https://www.facebook.com/notes/facebook-engineering/under-the-hood-the-entities-graph/10151490531588920/) for its users’ interests.

[Implementing a simple graph](https://www.geeksforgeeks.org/implementation-graph-javascript/) using a class.

[Details on the data structure.](https://medium.com/swlh/data-structures-graphs-50a8a032db03)

[Download GA’s Study Guide.](https://ga-waite.s3.amazonaws.com/production/sanitized-pdfs/distribution-and-descriptive-statistics-delete-421.pdf)


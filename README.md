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

![Image of Directed vs Undirected Graphs](data:image/png;base64,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)

* Undirected edges represent bidirectional connections, like a friendship on facebook.

* Directed edges represent an unidirectional connection, like a follow on instagram. For example, you may follow an account, but it will not necessarily follow you back.

#### What is the difference between a tree and a graph?

Trees are a subset of graph wherein all nodes are connected upward to a parent node. Graphs have no requirements on how connections (edges) work.
    Both Breadth-First and Depth-First searches may be utilized on graphs, but be sure to use a ‘visited’ boolean as Graphs may contain cycles (trees will not).

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


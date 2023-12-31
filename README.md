# Shortest Path Algorithms
### Devlin Ih, Sohum Kothavade, Natsuki Sacks

This repository contains all code files for the Discrete Math Group Deep Dive 1. Our group delved deeper into three of the most popular shortest-path algorithms: Dijkstra's, A*, and Bellman-Ford. 

**Shortest path algorithm:** used in graph theory; finds the "shortest path" between two nodes/vertices, meaning that the sum of the weights of the edges are minimized.

For our first Group Deep Dive (GDD), our group chose to further explore some of the well-known shortest path algorithms: **Dijkstra's, A-star (A\*)**, and **Bellman-Ford.** We chose to focus on the code implementation and visualization of these algorithms. To cater to our varying learning goals and coding abilities, we each coded a separate algorithm and made some sort of visualization for it. Suki delved deeper into Dijkstra's, Devlin did A\*, and Sohum did Bellman-Ford.

This repository introduces the reader to these three popular shortest path algorithms, assisting learning with the help of visualizations and real-life applications. To dive deeper into these algorithms and play around with the code implementations, explore each of the subfolders. 

## **Introducing the algorithms**
### **Dijkstra's Algorithm**
Dijkstra's algorithm is arguably the most well-known shortest path algorithm, working well with graphs that are not too complex, not bidirectional, and do not have negative weights.It is often used in network routing protocols.

Dijkstra's was conceived in 1956 by Edsger W. Dijkstra as a thought experiment on the fastest way to get to a certain location. It has many variants; the original algorithm found the shortest path between two given nodes, while other implementations chooses a single "source node" and finds the shortest path to all other nodes, effectively creating a shortest-path tree.

Explore our Dijkstra's implementation in [this subfolder.](./dijkstra)

### **A\***
A downside of A\* is its $O(b^d)$ space complexity, due to the fact that it stores all generated nodes in memory instead of pre-processing the graph. It is built off of Dijkstra's algorithm, with the addition of a heuristic. The heuristic function $h(t)$ estimates the distance of any given node to the destination node. Instead of producing a shortest-path tree like Dijkstra's, A* finds the shortest path from a specific source to a specific goal.

Explore our A* implementation in [this subfolder.](./a-star)

### **Bellman-Ford**
Bellman-Ford is similar to Dijkstra's in that it finds all shortest paths to each node from a defined source node (In fact, it runs Dijkstra's as a subroutine for the actual shortest path implementations). Although this algorithm is slower than Dijkstra's, it's more versatile since it's able to handle graphs with negative weights.

This algorithm states that all edges of an N vertex graph should be relaxed N-1 times to compute the shortest path from the source node. Relaxation works by continuously shortening the calculated distance between vertices comparing that distance with other known distances.

Explore our Bellman-Ford implementation in [this subfolder.](./bellman-ford)

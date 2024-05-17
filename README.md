# bangloreMetro

# Metro Navigation System

## Overview

This project implements a graph-based navigation system for a hypothetical metro network in Bangalore. It provides functionalities such as displaying all stations, showing the metro map, finding the shortest distance between two stations, and finding the shortest path (distance-wise) between two stations.

## Features

1. **Display all stations**: List all metro stations present in the network.
2. **Show the metro map**: Display the connections between stations with distances.
3. **Get shortest distance**: Calculate the shortest distance from a source station to a destination station.
4. **Get shortest path**: Provide the shortest path (distance-wise) from a source station to a destination station.

## Classes and Methods

### Graph_M

#### Inner Classes

- **Vertex**: Represents a vertex (station) in the graph. Each vertex has a hashmap of its neighboring vertices and the respective edge weights (distances).

- **DijkstraPair**: Used in the Dijkstra algorithm to store vertex name, path so far, and the cost to reach that vertex.

- **Pair**: Used for BFS traversal to store vertex name, path so far, minimum distance, and minimum time.

#### Methods

- **Graph_M()**: Constructor to initialize the graph.
- **numVertex()**: Returns the number of vertices in the graph.
- **containsVertex(String vname)**: Checks if a vertex is present in the graph.
- **addVertex(String vname)**: Adds a vertex to the graph.
- **removeVertex(String vname)**: Removes a vertex from the graph along with its edges.
- **numEdges()**: Returns the number of edges in the graph.
- **containsEdge(String vname1, String vname2)**: Checks if an edge exists between two vertices.
- **addEdge(String vname1, String vname2, int value)**: Adds an edge between two vertices with a given distance.
- **removeEdge(String vname1, String vname2)**: Removes an edge between two vertices.
- **display_Map()**: Displays the metro map.
- **display_Stations()**: Displays the list of all stations.
- **hasPath(String vname1, String vname2, HashMap<String, Boolean> processed)**: Checks if there is a path between two vertices.
- **dijkstra(String src, String des, boolean nan)**: Finds the shortest distance between two vertices using Dijkstra's algorithm.
- **Get_Minimum_Distance(String src, String dst)**: Finds the shortest path in terms of distance between two vertices.
- **Get_Minimum_Time(String src, String dst)**: Finds the shortest path in terms of time between two vertices.
- **get_Interchanges(String str)**: Finds the interchanges in the path.
- **Create_g_Map(Graph_M g)**: Initializes the graph with predefined stations and edges.
- **printCodelist()**: Prints the list of stations along with their codes.
- **getRoute(String src, String dst)**: Gets the shortest path between two vertices.

## Usage

### Running the Program

To run the program, compile and execute the `Graph_M` class. The program provides a menu-driven interface to interact with the metro navigation system.

### Menu Options

1. **List all stations**: Displays all the metro stations in the network.
2. **Show the metro map**: Prints the metro map with stations and their connections.
3. **Get shortest distance**: Allows you to input source and destination stations and calculates the shortest distance between them.
4. **Get shortest path (distance-wise)**: Provides the shortest path from the source station to the destination station.

### Example Usage

1. **List all stations**:
    ```
    1. LIST ALL THE STATIONS IN THE MAP
    ```
    This option lists all the stations in the metro network.

2. **Show the metro map**:
    ```
    2. SHOW THE METRO MAP
    ```
    This option displays the metro map with connections and distances between stations.

3. **Get shortest distance**:
    ```
    3. GET SHORTEST DISTANCE FROM A 'SOURCE' STATION TO 'DESTINATION' STATION
    ```
    This option allows you to input the source and destination stations and calculates the shortest distance between them using Dijkstra's algorithm.

4. **Get shortest path (distance-wise)**:
    ```
    4: GET SHORTEST PATH (DISTANCE WISE) TO REACH FROM A 'SOURCE' STATION TO 'DESTINATION' STATION
    ```
    This option provides the shortest path (distance-wise) from the source station to the destination station.

## Example Output

```
****WELCOME TO THE METRO APP*****
~~LIST OF ACTIONS~~

1. LIST ALL THE STATIONS IN THE MAP
2. SHOW THE METRO MAP
3. GET SHORTEST DISTANCE FROM A 'SOURCE' STATION TO 'DESTINATION' STATION
4: GET SHORTEST PATH (DISTANCE WISE) TO REACH FROM A 'SOURCE' STATION TO 'DESTINATION' STATION
5. EXIT THE MENU
```

## How to Contribute

Feel free to fork this project, make improvements, and submit a pull request. For major changes, please open an issue first to discuss what you would like to change.

## License

This project is licensed under the MIT License. See the LICENSE file for more details.

---

This README provides an overview of the project, its features, classes, methods, usage instructions, and an example of how to interact with the system. Feel free to modify it to suit your project's specific needs.

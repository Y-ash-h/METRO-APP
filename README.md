# OBJECTIVE:
Create a versatile routing system offering users various travel preferences:
Display all available paths for selection.
Optimize for maximum stations or minimum stations.
Find the shortest distance route.
Allow users to specify a mid-way station for personalized routes.
This system will employ advanced algorithms to process real-time transportation data, providing commuters with tailored, efficient travel options.

# KEY FEATURES:
## USER MANAGEMENT:
User registration and login functionalities with unique IDs and passwords.
Storage and retrieval of user details, including ID, password, and metro card balance.
## METRO STATION REPRESENTATION:
Representation of the Noida Metro system with stations connected through an adjacency list.
Displaying the stations in a structured format for easy use.


# PATH FINDING:
Algorithm to find all possible paths between a source and destination using Depth First Search.
Options to display shortest distance routes, paths with minimum/maximum stations or all available paths.
ROUTE SELECTION AND DETAILS:
User interface allowing users to select their source and destination stations.
Providing estimated distance, time and fare for selected routes based on preferences like:
All paths displayed for user selection.
Path with the maximum number of stations.
Path with the minimum number of stations.
Shortest distance route.
Ability for users to specify a particular station en route for personalized travel plans.

# METRO CARD MANAGEMENT:
Integration of Metro Card system for fare payments during travel.
Updating metro card balance based on travel fare and user interactions.
# FILE HANDLING:
Saving and loading user counts, user details and other relevant data in external files.
Utilising file I/O for persistent storage and retrieval of user related information.
CODE ORGANIZATION AND MODULARITY:
Usage of classes for stations and users.

# TOPICS USED:
##  C++ Language and Object Oriented Programming:
Classes and Objects: The program utilizes classes like station and user to encapsulate station details and user information, respectively.
Encapsulation: Data members (like stations map, idpassword, metrocardbalance) and member functions (like fare(), display(),
updatebalance()) are encapsulated within these classes to control access and maintain data integrity.
 Set (Data Structure):
Employed within the adjacency list (adjList) to represent connections between stations.
 ## Vector:
Used to store and manage paths between source and destination stations (allPaths).
 ## Map:
It's used to store station information, mapping station IDs to station names (metroSystem.stations)..


 ## Graph Data Structure:
Implements a graph data structure using an adjacency list, representing metro stations as nodes with edges connecting stations on the same metro line.
Adjacency List Representation:
The program uses an adjacency list to represent the metro system. The adjlist variable is an unordered map where each key represents a station, and the corresponding value is a set of pairs containing adjacent stations and their respective distances.
## Path Finding – Depth First Search:
The DFS algorithm is used to find all possible paths between a given source and destination station.
Within the findAllPaths() function, DFS is implemented using a stack to traverse through the graph, exploring all possible paths until the destination station is reached.
-The algorithm maintains a stack of visited nodes and backtracks
whenever it encounters a dead end until all possible paths are explored.

 ## Dijkstra's Algorithm:
The program also calculates the shortest distance between stations using Dijkstra's algorithm.
The shortestdistance() function utilizes a set to manage distances and applies a variation of Dijkstra's algorithm to find the shortest path from the source station to all other stations in the graph.


 ## File Handling:
- Employs file handling to store and retrieve user counts and user details in external files (‘usercount.txt’) and (‘userdetails.txt’).

CASE DIAGRAM

<img width="448" alt="image" src="https://github.com/user-attachments/assets/a909adf5-cdd8-403c-9caa-8794695acac5">





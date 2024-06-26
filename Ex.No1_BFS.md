
# Ex.No: 1  Implementation of Breadth First Search 
### DATE: 12/02/2024                                                                            
### REGISTER NUMBER : 212221040032 
### AIM: 
To write a python program to implement Breadth first Search. 
### Algorithm:
1. Start the program
2. Create the graph by using adjacency list representation
3. Define a function bfs and take the set “visited” is empty and “queue” is empty
4. Search start with initial node and add the node to visited and queue.
5. For each neighbor node, check node is not in visited then add node to visited and queue list.
6.  Creating loop to print the visited node.
7.   Call the bfs function by passing arguments visited, graph and starting node.
8.   Stop the program.
### Program:
```
graph = {
 '1' : ['2','3','4'],
 '2' : ['5', '6'],
 '3' : ['7','8'],
 '4' : ['9','10'],
 '5' : [],
 '6' : [],
 '7' : [],
 '8' : [],
 '9' : [],
 '10': []
 }
visited = [] 
queue = []     
def bfs(visited, graph, node): 
    visited.append(node)
    queue.append(node)
    while queue:
        m = queue.pop(0)
        print (m)
        for neighbour in graph[m]:
            if neighbour not in visited:
                visited.append(neighbour)
                queue.append(neighbour)
print("Following is the Breadth-First Search")
bfs(visited, graph, '1')
``` 




















### Output:

![bfs output](https://github.com/chgeethika/AI_Lab_2023-24/assets/142209368/af532e15-f020-4040-a8e0-024ae495b9b0)






### Result:
Thus the breadth first search order was found sucessfully.

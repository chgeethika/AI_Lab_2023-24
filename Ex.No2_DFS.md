# Ex.No: 2  Implementation of Depth First Search
### DATE: 12/02/2024                                                                           
### REGISTER NUMBER : 212221040032
### AIM: 
To write a python program to implement Depth first Search. 
### Algorithm:
1. Start the program
2. Create the graph by using adjacency list representation
3. Define a function dfs and take the set “visited” is empty 
4. Search start with initial node. Check the node is not visited then print the node.
5. For each neighbor node, recursively invoke the dfs search.
6. Call the dfs function by passing arguments visited, graph and starting node.
7. Stop the program.
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
visited = set() 
def dfs(visited, graph, node): 
    if node not in visited:
        print (node)
        visited.add(node)
        for neighbour in graph[node]:
            dfs(visited, graph, neighbour)
print("Following is the Depth-First Search")
dfs(visited, graph, '1')
```

### Output:
![Screenshot 2024-02-25 102926](https://github.com/chgeethika/AI_Lab_2023-24/assets/142209368/ae355b9e-d3c0-4994-8d22-0b42fe9e23b5)




### Result:
Thus the depth first search order was found sucessfully.

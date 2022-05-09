# Network-Vulnerablity

## How to run the code:

Download and unzip the code

Cd into the folder

And run this command:

```
g++ -o network .\NetworkVulnerability.cpp
```
 ```
./network 
```

# Project Description

A communication network is robust if it has alternative paths to mitigate failure in a 
node(vertex) or link(edge). A vertex is an articulation point/vertex if removing it and all the 
edges associated with it increases the number of connected components in the graph. The 
presence of articulation points/vertices in a graph representing a network indicates the 
presence of network vulnerabilities. This is because deleting an articulation point 
disconnects the network.



For instance, in Fig 1(a) vertex 3 is an articulation point. Edge (3,4) is a bridge edge. In Fig 
1(b), vertices 3 and 5 are articulation points. Edges (3,5) and (4,5) are bridge edges.



Required:

a) Write a program that identifies the following two vulnerabilities in an undirected graph:

• Articulation points/vertices

• Bridge edges

The program should not permit user interaction while executing.

b) Include program comments for internal documentation.

c) Describe your solution strategy and prepare a memory and space complexity analysis 
of your code (no more than half a page).

Input

The input will contain at least one test case. The first line of each test case will contain two 
integers: N(N≤100) and M, representing the number of vertices and the number of edges, 
respectively. Each of the next M lines will contain two integers v1 v2, where v1 and v2 are 
the vertex numbers that define an edge. Vertex numbers are positive integers ranging from 
1 to N. The input ends with two zeros for N and M. You can assume that all input is valid and 
contains no errors.

Input should be read from an input file input.txt



Sample Input

4 4

1 2

1 3

2 3

3 4

5 5

1 2

1 3

2 3

3 5

4 5

3 3

1 2

1 3

2 3

0 0

Output

Write your Andrew ID on the first line of your output file. For each test case in the input, 
print:

- The test case number. This should be an incrementing number starting from 1.

- A list of articulation vertices.

- A list of bridge edges, each made up of two vertices, ordered by the first vertex.


All the three items should be printed on a separate line. Print a blank line after the output 
for each test case. If any of the lists is empty, print “None”.

If you do not complete the implementation of any of the two vulnerabilities, print 
“Incomplete”. 
If you print “None”, implying that your program attempts to compute the list, 
for any incomplete implementation, this would be interpreted as a breach of the CMU Africa honour code, and you will be assigned a mark of zero for the entire assignment.
Output should be written to an output file output.txt.

Sample Output

mngongng

Test case: 1

Articulation points: 3

Bridge edges: (3,4)

Test case: 2

Articulation points: 3 5

Bridge edges: (3, 5) (4, 5)

4

Test case: 3

Articulation points: None

Bridge edges: None



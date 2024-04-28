# Max_Clique
How to run my code:
Download the sample graphs that I’ve provided. These are in the “G” folder
Download the MaxClique.py file
Edit the file variable at line 118. Edit this line to whatever graph file you want to run.
Run the python file. All the functions are already set up and called in the code. There is nothing else that needs to be done. 

Comments about my code:
First off, I used python to code this project. This is what I used for the TSP project, and I was able to reuse some code for that project. 
Additionally, I implemented all my functions using the adjacency matrix. This means that my code will not work for inputs that are adjacency lists.

Brute Force Algorithm:
For this algorithm, I used a recursive method to brute force the Max Clique. This code is incredibly slow compared to the other algorithms that I coded, but I’m pretty sure that I get the correct answer from the code.
The functions that are associated with the Brute force algorithm are:
construct_graph(name)
is_clique(v, n)
BF_max_clique(startV, size)

Solver Algorithm:
For this algorithm, we were instructed to create a solver that pretty much finds the vertex cover of the complement graph. By finding the vertex cover of the complement graph, that same answer is the Max Clique of the original graph. This is due to the reduction that was created by really smart computer science people. Although I tried my best to code the algorithm, the code to find the vertex cover is just not right. I think it’s close, but it is just not right at all. This means that the answer is not even close to right, but the logic is sound with the structure of my code. 
The functions associated with the solver are:
construct_graph(name)
construct_complement_graph(file)
vertex_cover(matrix)
MC_from_VC(file)

Competitive Algorithm:
For this algorithm, I decided to implement a greedy algorithm that solves the max clique problem. The implementation is pretty trivial and it follows a greedy strategy. This code doesn’t give you a very accurate answer, but it is fast and gives you an answer that is close. It’s a heuristic that prioritizes speed over accuracy. 
Associated functions:
G_max_clique(matrix)

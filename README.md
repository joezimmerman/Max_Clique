# Max Clique Solver

## How to run my code:
1. Download the sample graphs provided in the "G" folder.
2. Download the MaxClique.py file.
3. Edit the `file` variable at line 118 to point to the graph file you want to run.
4. Run the Python file. All necessary functions are already set up and called in the code.

## Comments about my code:
- I used Python for this project, leveraging some code from the TSP project.
- All functions are implemented using the adjacency matrix, making the code incompatible with adjacency lists.

## Brute Force Algorithm:
- I employed a recursive method for the Brute Force Max Clique algorithm. Although slow, I believe it produces the correct results.
- Functions:
  - `construct_graph(name)`
  - `is_clique(v, n)`
  - `BF_max_clique(startV, size)`

## Solver Algorithm:
- The solver attempts to find the vertex cover of the complement graph, which corresponds to the Max Clique of the original graph due to a reduction. However, the vertex cover calculation is flawed, resulting in inaccurate results.
- Functions:
  - `construct_graph(name)`
  - `construct_complement_graph(file)`
  - `vertex_cover(matrix)`
  - `MC_from_VC(file)`

## Competitive Algorithm:
- Implemented a greedy algorithm for solving the Max Clique problem. This approach prioritizes speed over accuracy, providing a fast but approximate solution.
- Associated functions:
  - `G_max_clique(matrix)`

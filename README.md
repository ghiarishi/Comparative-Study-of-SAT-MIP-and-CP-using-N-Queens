# Comparative-Study-of-SAT-MIP-and-CP-using-N-Queens

This project primarily deals with comparing each, SAT, MIP and CP by solving the N-Queens problem using each. I shall compare them on the basis of their: 
a. Runtime and order of growth
b. Number of constraints required
c. Improvements possible through heuristics 
d. Time taken to calculate all valid solutions


Execution: 
•	The first step shall be to create the solvers, while using appropriate metrics to evaluate how each solver performs.

•	Runtime and order of growth can be determined through the ‘Doubling Method’, where we shall keep doubling the input size to our algorithms, and note down their respective runtimes. 

•	Once we have solved the problem at a basic level using each of these techniques, we shall try to come up with heuristics in order to improve each of them. If we succeed in the above, we shall compare what the improvements obtained with those respective heuristics are. 

•	Further, once the code to solve one instance of the problem is optimized, we shall attempt creating a solver to output all valid solutions to the given input. We believe that each technique will perform differently while calculating all valid solutions, and we plan to document that.

•	It was found that the time taken by the MIP Solver increases at a very fast rate, and for large values of n > 8, the time taken crossed 5 minutes, making it impractical for comparison (This is believed to be due to the exponentially increasing number of constraints).

•	In order to get around such issues, we implemented several heuristics in each of the solvers, to make it possible to calculate runtime metrics for n's greater than 15. 

Results: 

• Order of Growth: O(𝑛^𝑛)

• MIP is the slowest amongst the three, with SAT being the fastest

• CP-SAT’s “SearchForAllSolutions” takes 20 seconds for n = 12 (making it the fastest), while our solver to find the fundamental solutions takes over 5 minutes for the same

• 14x improvement for n = 8 achieved through heuristic in MIP

![image](https://user-images.githubusercontent.com/72302800/200106795-5dc58a51-65c4-431b-8bf1-3cb2f143c92b.png)

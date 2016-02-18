Learning to Brnach in MIP (E. Khalil et al)

Machine learning approach for speeding up MILPs:
    * Look at branch and bound
    * How to brnach efficiently?
    * Compute the quality of the branch

Common brnaching strategies:
    * Strong branching: simulate brnaching factor at each node (requires LP solution)
    * Pseudocost Branching: keep running average for each branching

Approach:
    * Learng the ranking model of each variable at each node
    * Incorporate directly into the MIP solver (on the fly approach)
    * Instance specific, b/c learns on the fly specific to problem (kind of like AlphaGo)
    * Use atomic and interaction features: can compute these efficiently?
    * Scale features [0,1]
    * Use 72 atomic features :O and 54 dynamic features
    * Label [0,1] - relaxed binary labels
    * Use learning to rank with pairwise costs to train (convex SVM problem)

Results:
    Solve more instances and solve hard instances faster

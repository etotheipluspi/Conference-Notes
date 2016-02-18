Deep MPC:

Focus on the food cutting problem: 
    * No info about object
    * Cut through object
    * Stop when hit cutting board

Previous work:
    * Stiffness controller: compare current trajectory to target trajectory
    * Problem is that knife gets stuck

Problems:
    * Complex dynamics
    * Coupled dynamics
    * Variation in food cutting dynamics
        - Thickness, rigidity, etc
        - Need to tune controllers for each class

Deep Learning:
    * Use deep learning to learn dynamics to be used MPC
    * Use RNNs and conditional modal in combinations
    * use incremental training?

Benefits:
    * Don't need to engineer dynamics features
    * Fast forawrd compute time
    * Quick prediction step in MPC

Plans to use POMDP-like model

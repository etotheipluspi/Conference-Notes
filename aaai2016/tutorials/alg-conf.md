AC: Essentially Hyperparameter tuning

Solving an optmization problem: which (hyper-)parameters give you the best results on cost metric (time, performace, memory etc)

General framework: for ML, SAT, Tree Search, etc

Applications:
* Parameters for SAT instances
* Best fold in K-fold cross validation
* When comparing approaches to other algorithms that we dont know well
    - Are our MPC algorithms optimized? Not sure because we only know about POMDPs :p


Why is this important: automatic parameter tunning
Slide 17 [here](http://www.ml4aad.org/wp-content/uploads/2016/02/AC-Tutorial.pdf).

Example case: deep learning
    - Good for automatically learning features BUT
    - Very sensitive to hyperparameters

Have a few rules of thumb:
    * Use good default params...
    * Use > 1000 instances for training
    * ~75% of 'easy' instances in the trianing set (these are solvable by default params

Follow these, and can usually find better parameters

Limitations:
    * SpySMAC can only do runtime optimization, cant use for MDP/POMDP policy evaluation :(

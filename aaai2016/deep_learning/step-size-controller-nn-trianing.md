
Can we use RL to replace expert?

RL for hyper parameter tunning?? -> Only step size

What is the state space (features to consider):
    * Variance of function values (loss?)
    * Vriance of changes of function values (need to predict -> use Taylor expansion)

Use RL to train controller using above features as state space -> both vars are continues, cant just use Q-learning

Questions:
    * Is controlelr robust to initalization
    * Does it transfer

Experiment:
    * Subset of MNIST to train controller
    * Use controller on a bigger network with full data set (changed the architecture)
    * Used same controller on CIFAR
    * Fails when they change update method



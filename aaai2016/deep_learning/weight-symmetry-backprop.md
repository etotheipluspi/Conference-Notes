How Important is Weight Symmetry in Backprop? Liao et al

What is backprop in the model of brain? Is backprop biologically plausible?

Can the brain implement backprop or some variance?

Previous work: NO
    * Feedback weight and feedback weights must be same
    * Back and forward prop require different computations -> cant in brain
    * Error gradients must be stored somewhere  b/c neurons already storing activations

Cant implement backrpop with two neurons...

Naive solution:
    * Have an identical set of neurons that stores gradient error
    * Dont need exact errors in backprop to still train the wieghts
    * Brain could implement this?
    * Can make backprop work on two netowrks with slightly different grad errors with batch norm
    * Two networks one for forward and backward compute

How different can the two netowrks be?
    * V and W are the two grads of the two netowrks
    * V = M * sign(W) * Sp (M and Sp are rand)
    * Robust to sign() and -1 1 mul factor
    * Need batch norm!

Is batch norm bio plausible? Synnaptic scaling in brain may be like backprop 

POMDP Formulation for Proactive Learning (K.H. Wray et al)

Motivation:
    * Build active learning model of a classifier
    * Determine at risk people during disease outbreak
    * May have noise when getting training data (are the trianing labels correct? - not always)

POMDP formulation:
    * State: # correct labels, # wrong labels, # last oracle responded? 
    * Ex: (3,2,T), 3 correct, 2 wrong, last oracle responds
    * Belief over accuracy of data set labels
    * Actions: which oracle should label the data point
    * Obs: if oracle responded or not?

Problem structure:
    * Reachable beliefs non-zero on sqrt(n) states -> so point based methods work well






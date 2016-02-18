X. Jin et al
S-shaped ReLU

ReLU, LReLU, Maxout cant learn non-convex functions (does this matter if you have multi-layer netowrks?)

Motivated by psychophysics: relation between physical stimulas and its perceived intensity and srength
    * Whener Law (log)
    * Power Law

SReLU:
    * Linear comb of Three linear functions
    * Can approx both the log and power functions (and convex functions)
    * Need a few more params: Inception (5mb) + 21kb if replace all ReLU with SReLU 
    * Needs parameter initialization: non-trivial, bad initialization breaks training
    * Propose adaptive initialization -> Use LReLU here??

Some experiemnts on CIFAR, MINST and ImageNET (outperforms standard architectures on all)

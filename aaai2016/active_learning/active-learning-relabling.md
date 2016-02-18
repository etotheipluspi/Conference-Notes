Re-active learning (C.H. Lin, et al)

How to correctly re-label training data?

Currently:
    * Multiple labelers and with most common label
    * Balance: more noisy data vs less better data (which is more impartant?)

Contributions:
    * Standard approachs (uncertainty sampling and expected error reduction fail)
    * Propose new approach (generalization of ...)

Naive Approach:
    * Look at the number of labels on each sample and weigh sample according to uncertainity (extension of uncertainity sampling)
   
Impact sampling (main contribution):
    * Measure impact of labeling a sample in expectation
    * Use Bayes rule to update impact (prob of impact)
    * Assume annotation accuracy > 0.5 ?? what does this mean? over half the samples are correctly labeled?






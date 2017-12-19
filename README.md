# taa
Temporal Alignment Algorithm for UCR classification

This repository contains the codes for the TAA algorithm and pruning techniques proposed in ECML PKDD 2018.

The TAA algorithm is a temporal sequence alignment algorithm which has two hyperparameters: a static gap penalty, g, and a temporal penalty weight, w.
When w = 0, the alignment can be computed using the Needleman-Wunsch algorithm using the value of g.

- TAA_banded.java: contains the code for the TAA algorithm.  The code allows you to use a k-band around the diagonal which can be used to limit the matrix computation as discussed in the paper.
- NW_timing.java: contains an adaptation of the Needleman-Wunsch algorithm for time series.  The method returns the NW score for the time series given that the "match" case incurs a score equal to the norm of the values being compared.  The method returns a second output which is the post-hoc timing penalty.  The timing penalty is computed in O(n) after computing an alignment by comparing the timings of the alignmed time series as discussed in the paper.

# taa
Temporal Alignment Algorithm for UCR classification

This repository contains the codes for the TAA algorithm and pruning techniques proposed in ECML PKDD 2018.

The TAA algorithm is a temporal sequence alignment algorithm which has two hyperparameters: a static gap penalty, g, and a temporal penalty weight, w.
When w = 0, the alignment can be computed using the Needleman-Wunsch algorithm using the value of g.

- TAA.java: contains the code for the TAA algorithm
- NW.java: contains the Needleman-Wunsch algorithm

The repository is being updated and the algorithms will be posted in a week.

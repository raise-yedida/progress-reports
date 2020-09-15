

# Progress Summary (Sep 11 - Sep 18)

## Issue close time

| Result                                            | Elaboration                                                  |
| ------------------------------------------------- | ------------------------------------------------------------ |
| GHOST non-DL < DODGE < GHOST-DL                   | GHOST on non-DL learners performs *worse* than regular DODGE in some cases; at best, it ties with GHOST, but never wins. Therefore, weighted losses help, but only DL can do well with WFO. |
| No comparable prior SOTA for issue close times    | The only [other one](https://ieeexplore-ieee-org.prox.lib.ncsu.edu/stamp/stamp.jsp?tp=&arnumber=7832909), used in the Mitch study, report only AUC and F-1 scores, and their GitHub does not have pf and recall numbers. |
| GHOST with round robin on issue close time is bad | It has worse performance, and also runs significantly slower. |


# April 8 - April 15 Progress Report

## Doing

* **DODGE:**
    * Modified code a bit, running DODGE on defect prediction.
    * Probably needs more tweaking
    * On lucene defect prediction data, Amrit's AUC *seems to be* between 37.656 and 54.846 (from `d2h_lucene.pickle`), which DL is in upper 60s (currently running).

## Done

* **March deliverable:**
    * Completed: added text to Overleaf document with figure of high-level and low-level operations.
* **Baseline results:**
    * Got baseline results with new metrics.
    * Need to train on better loss functions

## Todo

* Run DODGE on others, preferably on ARC

## Roadblocks

* Cannot run code on ARC:
    * Cannot install required modules, but pip does not exist
    * Cannot install pip without root access on CentOS
* Heavy project work for 540, midterm for 505 on Wed Apr 15
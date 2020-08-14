# Progress Summary (Aug 7 - Aug 14)

## Doing

* **RAISE:**
    * Write tests

## Done

* **GHOST:**
    * Submitted TSE paper (yay!)
    * Updated [repo](tiny.cc/ghost-dl)
    * Possibly found source of GHOST power: weighted fuzzy oversampling. [spreadsheet](https://docs.google.com/spreadsheets/d/1rRPnKvuwTste6WA98z7qRV-e9PWejTzouk_fwA6WnlU/edit?usp=sharing) 
        * therefore, ran wfo on classical learners: [spreadsheet](https://docs.google.com/spreadsheets/d/1D3JGBYe-BHOBfsKNv5qET15ioew_SpWuIwATr07giMc/edit?usp=sharing) | [data](https://drive.google.com/drive/folders/1bp3VIRg1bTn5DT4q7nfBU8tHbbcWkjWV?usp=sharing) 
            * hypothesis is true:
                * NB is **worse** with with WFO (**expected**), because it assumes $p(x|y=0)$ and $p(x|y=1)$ are Gaussian, but (a) they likely are not (b) wfo only exacerbates (a).
                * Logistic regression is **worse** with WFO (**expected**), because it assumes the residuals $w^T x - y$ follow a normal distribution--this may not be true; wfo exacerbates this issue.
                * Decision tree learners are a mixed bag (**unexpected**): they assume rectangular partitions exist; when they do, wfo helps; when they don't wfo makes things worse.
                * Random forest does **better** with WFO (**expected**): because it follows boosting, the random splits + boosting are helped by the robust decision boundaries that wfo helps create.
        * and also compared regular, weighted, weighted + wfo classical learners. [spreadsheet](https://docs.google.com/spreadsheets/d/1A9cW7teQB0m7oXst-a0kTei1rqZeyST9R_p57qHT0sg/edit?usp=sharing) | [data](https://drive.google.com/drive/folders/1KmEmFmQNaifhnsn8C3Rq5hMvb1CctPRJ?usp=sharing) 
* **RAISE:**
    * Updated package and documentation
* **DL thesis:**
    * Made notes, found their feature extraction code, some ideas, found code to encode code.

 
# Aug 21 - Sep 4 Progress Summary

## Done

* **DL4SE:**
    * Literature review complete | [Google sheet](https://docs.google.com/spreadsheets/d/1iaUiecliRFzhj0Hff1vNR2JonrKMDKun0SVH2OB-CCU/edit?usp=sharing) | [overview](https://github.com/yrahul3910/dl4se/blob/master/lit-review/results.md) 
    * Heatmap generated | [link](https://github.com/raise-yedida/progress-reports/blob/master/2020/Aug%2021%20-%20Sep%204/heatmap.png)
* **Weighted losses:**
    * Ran non-DL (untuned) with all treatments on issue close time data (56 datasets) 
        * *Non-DL only:* [table on Overleaf](https://www.overleaf.com/9879323264fpnhvbtjhbjx) | [table pdf](https://github.com/raise-yedida/progress-reports/blob/master/2020/Aug%2021%20-%20Sep%204/table.pdf) | [pie charts](https://github.com/yrahul3910/nondl-wfo/blob/master/nondl-only-results.md) | [raw Scott-Knott numbers](https://github.com/yrahul3910/nondl-wfo/blob/b6906efa2361ebd4edd7572335a7209cf75764af/sk.txt) 
        * *Non-DL + DL:* [table on Overleaf](https://www.overleaf.com/9879323264fpnhvbtjhbjx) | [table pdf](https://github.com/raise-yedida/progress-reports/blob/master/2020/Aug%2021%20-%20Sep%204/table.pdf) | [pie charts](https://github.com/yrahul3910/dl4se/blob/master/issue_close_time/ghost/nondl-and-dl.md) | [raw Scott-Knott numbers](https://github.com/yrahul3910/dl4se/blob/master/issue_close_time/ghost/sk-full.txt) 
    * Ran modified version of GHOST on issue close time data
        * Bad idea; the original paper's defaults work MUCH better (e.g. `pd, pf=(1., 1.)` vs `pd, pf = (0.83, 0.01)`). Re-run?
* **RAISE package:**
    * Added more stuff, some ironing out

## Doing

* **Weighted losses:**
    * Running GHOST with both variants of weighted fuzzy oversampling on issue close time data
* **RAISE package:**
    * Polishing it up

## Todo

* **RAISE package:**
    * Fix issues
    * Add more tests
* **Issue close time:**
    * After code done running, (a) run Scott-Knott to compare the weighted schemes (b) compare with Mitch using point statistics
# Aug 21 - Sep 4 Progress Summary

## Done

* **DL4SE:**
    * Literature review complete
    * Heatmap generated | [link](https://github.com/raise-yedida/progress-reports/blob/master/2020/Aug%2021%20-%20Sep%204/heatmap.png)
* **Weighted losses:**
    * Ran non-DL (untuned) with all treatments on issue close time data (56 datasets) | [table](https://www.overleaf.com/9879323264fpnhvbtjhbjx) | [pie charts](https://github.com/yrahul3910/nondl-wfo/blob/master/Pie%20charts%20of%20results%20and%20table%20generation.ipynb) 
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
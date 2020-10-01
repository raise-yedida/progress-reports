# Progress Summary (Sep 23 - Oct 7)

## Executive Summary

* [Paper](https://www.overleaf.com/project/5f6557a43067ea000151dd57): work-in-progress (30%)
* **Literature review** update on DL4SE: 50% done, identified 36 new papers but needs filtering before adding to review
* [Replicating issue close time SOTA](https://github.com/yrahul3910/dl4se/tree/master/issue_close_time/DASENetComparison/Reproduction/DeepTriage): Could not replicate SOTA; was able to replicate #2.
* [Issue close time](https://github.com/yrahul3910/dl4se/blob/master/issue_close_time/DASENetComparison/PROMISE.ipynb): Working on establishing a baseline on a recently released dataset in PROMISE '19 (easy citations if we are the benchmark).
* RAISE package is live!

## Assistant-to-the-regional-manager Summary

* [Paper](https://www.overleaf.com/project/5f6557a43067ea000151dd57)
    * Work-in-progress
* [Literature review update on DL4SE] : (TODO: Add link)
    * 17/36 papers in the AI for V&V literature review
    * Next step: apply filter criteria and remove tangential papers
    * Then: update Excel file
* [Replication of issue close time SOTA](https://github.com/yrahul3910/dl4se/tree/master/issue_close_time/DASENetComparison/Reproduction/DeepTriage)
    * **DASENet** (SOTA): could not replicate results
        * Their code uses files that they do not publish, therefore cannot run it
        * On writing our own code using the specification from paper, (a) differs from the model they got from their code (b) performs very poorly
    * **DeepTriage:** Replicating with partial success
        * Combined datasets they used with DASENet data to get working code, results are within error bounds of reported values in DASENet paper. 
        * Need to run on more datasets
* [Established benchmark on PROMISE data](https://github.com/yrahul3910/dl4se/blob/master/issue_close_time/DASENetComparison/PROMISE.ipynb)
    * Paper very recently published, therefore no papers established benchmarks on this dataset.
* [RAISE package](https://github.com/yrahul3910/raise)
    * [Published documentation online at Read The Docs](https://raise.readthedocs.io/en/latest/)
    * [Published to PyPI](https://pypi.org/project/raise-utils/)

## Todo

* Complete paper
* Continue with literature review
* Finish replication
* Finish establishing baseline


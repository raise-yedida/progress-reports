# Progress Summary (Sep 23 - Oct 7)

## Executive Summary

* [Paper](https://www.overleaf.com/project/5f6557a43067ea000151dd57): work-in-progress (30%)
* [Literature review](https://docs.google.com/spreadsheets/d/1iaUiecliRFzhj0Hff1vNR2JonrKMDKun0SVH2OB-CCU/edit?usp=sharing) update on DL4SE: done - identified 3 new papers
* [Replicating issue close time SOTA](https://github.com/yrahul3910/dl4se/tree/master/issue_close_time/DASENetComparison/Reproduction/DeepTriage): Could not replicate SOTA; was able to replicate #2.
* [Issue close time](https://github.com/yrahul3910/dl4se/blob/master/issue_close_time/DASENetComparison/PROMISE.ipynb): Working on establishing a baseline on a recently released dataset in PROMISE '19 (easy citations if we are the benchmark).
* [RAISE package](https://pypi.org/project/raise-utils/) is live!

## Assistant-to-the-regional-manager Summary

* [Paper](https://www.overleaf.com/project/5f6557a43067ea000151dd57)
    * Work-in-progress
* Literature review update on DL4SE: [Updates](https://docs.google.com/document/d/1MRDrmY-LzU5dQWMuUT2wwYPRVvcEkmEjx_KyzlRin7k/edit?usp=sharing) | [Updated spreadsheet](https://docs.google.com/spreadsheets/d/1iaUiecliRFzhj0Hff1vNR2JonrKMDKun0SVH2OB-CCU/edit?usp=sharing)
    * 2/5 papers in the AI for V&V literature review
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
* Finish replication
* Finish establishing baseline


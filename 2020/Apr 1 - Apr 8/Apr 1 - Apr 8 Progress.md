# Apr 1 - Apr 8 Progress

## Doing

* Working on [Google sheet](https://docs.google.com/spreadsheets/d/1ffMFZ2A10wEdqtJDm-ADXCOIHCf8fLnQs1M0VuPyxnQ/edit?usp=sharing)

## Done

* **DODGE:** 
    * discussed code with Sherry to figure out what goes where
    * went through DODGE code, figured out potential optimizations
        * From paper, DODGE is stable across epsilon values. Experimentally, 0.2 works best. Therefore, we chose 0.2.
        * Need not seed with random algorithms; instead, seed with intuitive guesses.
* **Baseline results:**
    * [Text mining](https://github.com/ai-se/ai-for-vv/blob/master/rahul/Apr%201%20-%20Apr%208/text-mining/Text%20mining%20DL%20baseline.ipynb):
        * pitsA (4 classes): 64.38%
        * pitsC (6 classes): 88%
        * pitsD (5 classes): 85.71% 
* **March deliverable:**
    * Updated [Google sheet](https://docs.google.com/spreadsheets/d/1ffMFZ2A10wEdqtJDm-ADXCOIHCf8fLnQs1M0VuPyxnQ/edit?usp=sharing)

## Todo

* Find d2h, popt, and popt20 metrics for text mining.
* Run DODGE on deep learners

## Roadblocks

How to put the spreadsheet in the Overleaf doc (format, colors, etc.)
# Progress Report (Jul 1 - Jul 8, 2020)

## Doing

## Done

* Compared GHOST against other baselines
    * beats DODGE, as in [Excel sheet](https://oitncsu-my.sharepoint.com/:x:/g/personal/ryedida_ncsu_edu/Ed28oa7Y-zVDqogvMIlwmKwB5-XAPSmvdZXx6OQQ5vMBzQ?e=KC9Eyz)
    * loses against [Lin Tan's results](https://www.cs.purdue.edu/homes/lintan/publications/deeplearn-icse16.pdf) (wins in 2/10 datasets on recall)
        * **Q:** unsure if I should run GHOST for precision and compare, same for F1 score
* Ran modified version of SVM: [results](https://docs.google.com/spreadsheets/d/1aqjnF0hrnykLpAYEXMmrN_zAMaFu495f9ObYjwZ7ZcQ/edit?usp=sharing) | [code](https://github.com/yrahul3910/biased-svm/blob/master/Biased%20SVMs%20with%20weighted%20fuzzy%20oversampling.ipynb) | [theory](https://github.com/yrahul3910/biased-svm/blob/master/theory.pdf)
    * When tuned, beats DODGE in recall,  has only one hyperparameter to tune (therefore tuning is fast), but achieves good precision in 5/10 datasets, and matches DODGE in popt20 in all
        * advantage over DODGE: one single learner with one hyperparameter means runtime << DODGE
    * Also applied kernel: surprisingly, linear kernel works better than rbf; possibly because:
        * SE data is low dimensional, but the rbf kernel projects to an infinite-dimensional space
        * the k hyperparameter is lost in the projection and therefore is now redundant
* Implemented tab domination for [DANCE](https://github.com/yrahul3910/dance)
* [Baselines for issue close time](https://docs.google.com/spreadsheets/d/1ug-pR1S5Puxq9gun9w5QJBC8OA9I1HrqWdL6r-zoYPU/edit?usp=sharing) (AUC): ran DL and DODGE

## Todo

* Run [FFT baselines](https://github.com/ai-se/FFT_Jack/blob/master/issue_close_time_main.py) on issue close time
* Compare results between DL, DODGE, FFT
* Get DODGE pf results

## Roadblocks

* Did not understand the data or results in [Kikas paper](https://kodu.ut.ee/~dumas/pubs/msr2016IssueLifetime.pdf); [their code](https://github.com/reesjones/issueCloseTime) is mostly Bash and some Java + Weka
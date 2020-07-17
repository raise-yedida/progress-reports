# Jul 8 - Jul 23 Progress Summary

## Done

* **ICSE paper:**

    * Ran DODGE and DL on pits datasets | [raw spreadsheet data](https://docs.google.com/spreadsheets/d/108kxQa30gswWe2pJAoEz3XrWgEFwAb-xUAqnDFI45V0/edit?usp=sharing)

    <img src="./AUC vs L1 intrinsic dimensionality.png" width="23%"></img> <img src="./F1 score vs intrinsic dimensionality.png" width="23%"></img> <img src="./pf vs intrinsic dimensionality.png" width="23%"></img> <img src="./Recall vs intrinsic dimensionality.png" width="23%"></img> <img src="./AUC vs number of samples.png" width="23%"></img> <img src="./F1 score vs number of samples.png" width="23%"></img><img src="./pf vs number of samples.png" width="23%"></img><img src="./Recall vs number of samples.png" width="23%"></img> 

* **GHOST:**

    * Recall improved when using weighted fuzzy oversampling; plain GHOST loses to DODGE | [spreadsheet](https://oitncsu-my.sharepoint.com/:x:/g/personal/ryedida_ncsu_edu/Ed28oa7Y-zVDqogvMIlwmKwB5-XAPSmvdZXx6OQQ5vMBzQ?e=EV5gY6) 

## Ideas

### Working

* **Weighted fuzzy oversampling:** [code](https://github.com/yrahul3910/yedida-gone-nuts/blob/master/Biased%20SVMs%20with%20weighted%20fuzzy%20oversampling.ipynb) 

    * Definitely has potential to work, as shown by biased SVM and DNN--to the extent that biasing against was needed
    * Currently uses a primitive scheme, can improve using statistics of the data

* **Knowledge distillation:** [code](https://github.com/yrahul3910/yedida-gone-nuts/blob/master/Knowledge%20distillation.ipynb) | [paper](https://www.cs.cornell.edu/~caruana/compression.kdd06.pdf) 

    * Implemented, works (below is on a random neural network, with no effort in hyperparameter tuning).

        ```
        Teacher:
        ========
        Recall: 0.675
        AUC: 0.7445512820512821
        
        Student:
        ========
        Recall: 0.725
        AUC: 0.7631410256410257
        ```

    * Surprisingly, ensembles didn't work (or I didn't try hard enough)

        * This would suggest that you should spend your effort finding a really good deep learner, however complex, and then distill it. Perhaps use NAS? Hierarchical approach to NAS sounded exciting

### Will work if improved

* **Model trees:** [code](https://github.com/yrahul3910/yedida-gone-nuts/blob/master/model-trees/decision_tree.py)
    * Idea that different learners are used at different regions
    * Needs better split and stopping criteria

### Don't work

* **Committee of models:** [code](https://github.com/yrahul3910/yedida-gone-nuts/blob/master/Committee%20of%20models%20(doesn't%20work).ipynb)
    * Implemented, does not work, partially due to many classifiers at 0.5


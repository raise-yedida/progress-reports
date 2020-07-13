# Jul 8 - Jul 23 Progress Summary

## Doing

* **GHOST:**
    * Running models on ARC

## Done

* **ICSE paper:**

    * Ran DODGE and DL on pits datasets | [raw spreadsheet data](https://docs.google.com/spreadsheets/d/108kxQa30gswWe2pJAoEz3XrWgEFwAb-xUAqnDFI45V0/edit?usp=sharing)

    <img src="./AUC vs L1 intrinsic dimensionality.png" width="23%"></img> <img src="./F1 score vs intrinsic dimensionality.png" width="23%"></img> <img src="./pf vs intrinsic dimensionality.png" width="23%"></img> <img src="./Recall vs intrinsic dimensionality.png" width="23%"></img> <img src="./AUC vs number of samples.png" width="23%"></img> <img src="./F1 score vs number of samples.png" width="23%"></img><img src="./pf vs number of samples.png" width="23%"></img><img src="./Recall vs number of samples.png" width="23%"></img> 

## Todo



## Ideas

* **Weighted fuzzy oversampling:** [code](https://github.com/yrahul3910/yedida-gone-nuts/blob/master/Biased%20SVMs%20with%20weighted%20fuzzy%20oversampling.ipynb) 

    * Definitely has potential to work, as shown by biased SVM and DNN--to the extent that biasing against was needed
    * Currently uses a primitive scheme, can improve using statistics of the data

* **Model trees:**

    * Idea that different learners are used at different regions
    * How to define boundaries of regions?

* **Committee of models:** [code](https://github.com/yrahul3910/yedida-gone-nuts/blob/master/Committee%20of%20models%20(doesn't%20work).ipynb)

    * Implemented, does not work, partially due to many classifiers at 0.5

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

        * This would suggest that you should spend your effort finding a really good deep learner, however complex, and then distill it. Perhaps use NAS?


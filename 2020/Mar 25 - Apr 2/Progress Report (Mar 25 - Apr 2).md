# Progress Report (Mar 25 - Apr 2)

## Doing

* Baseline results for text mining with deep learning

## Done

* **Questionnaire: ** 
    * better organization
    * created [Google Form](https://docs.google.com/forms/d/1dZ9mb_-oFuI2WS_9had78CwFs7Ra0lQdUvPlXVkgwoM/edit?usp=sharing)
* **March [SBIR deliverable](https://www.overleaf.com/9581451812jgbhxfmjwwfc): ** 
    * added graphics
    * added problem at beginning of each subsection
    * wrote introduction and abstract
* Matrix of high-level operations (rows) vs. low-level methods to implement them (columns): [Google sheet](https://docs.google.com/spreadsheets/d/1ffMFZ2A10wEdqtJDm-ADXCOIHCf8fLnQs1M0VuPyxnQ/edit?usp=sharing).
* Found Amrit's results on DODGE from [his repo](https://tiny.cc/dodge2020). His results are below.

### Text mining

| **Dataset** | min(d2h) |
| ----------- | -------- |
| pitsA       | 0.351    |
| pitsB       | 0.707    |
| pitsC       | 0.088    |
| pitsD       | 0.105    |
| pitsE       | 0.22     |
| pitsF       | 0.356    |

### Defect prediction

| Dataset  | min(d2h) | max(popt) | max(popt20) |
| -------- | -------- | --------- | ----------- |
| ivy      | 0.325    | 0.604     | 0.336       |
| camel    | 0.474    | 0.731     | 0.529       |
| jedit    | 0.317    | 0.735     | 0.466       |
| log4j    | 0.48     | 0.782     | 0.989       |
| lucene   | 0.331    | 0.791     | 0.802       |
| poi      | 0.232    | 0.759     | 0.744       |
| synapse  | 0.456    | 0.605     | 0.478       |
| xalan    | 0.361    | 0.838     | 1.0         |
| velocity | 0.341    | 0.819     | 0.677       |
| xerces   | 0.585    | 0.871     | 0.944       |

## Todo

* Run FLASH/DODGE on DL for defect prediction

## Roadblocks

* Need to understand how to add deep learning code to DODGE code with Sherry
* Not sure what metric to use to evaluate deep learners on text mining, and what the output integers are (2-5)
# Pert-Analysis-with-Python

_Made by [@DanteSc03](https://github.com/DanteSc03) and [@migueldiazpdj](https://github.com/migueldiazpdj)_

This repository contains a Python implementation of the Program Evaluation and Review Technique (PERT), a widely used tool in project management for planning and scheduling tasks. We made this work for the subject of optimization for business analytics in order to analyze and understand the method and to be able to calculate an example.

## How to Use ❓

1. Define your tasks and their optimistic (o), pessimistic (p), and most likely (m) time estimates.
2. Define the dependencies between the tasks.
3. Run the `pert` function to get the analysis results.
4. The `Pert.py` file is intended to be a comprehensive example.
5. Running `pert` in `Pert-Interactive.py` allows you to customize your tasks, the quantity of tasks and the dependencies.

## Requirements
Run in the command line
```python 
pip install pandas
```
Pandas is necessary to run the files in this respository

```python
brew install graphviz
```
graphviz is required to create the graph within this repository

## Code Example

#### For Pert-Interactive.py
```python
import math
import pandas as pd

def pert(tasks, dependencies):
    # ... [Include the entire PERT function code here]

# Example usage
tasks = {
    # This dictionary is set to blank. When running the program, python will 
    # ask you to complete this information in the command line
}

dependencies = {
    # This dictionary is set to blank. When running the program, python will 
    # ask you to complete this information in the command line
}

results = pert(tasks, dependencies)

#Print the results
results_df = pd.DataFrame.from_dict(results, orient='index')
print(results_df)
```

#### For Pert.py
```python
import math
import pandas as pd

def pert(tasks, dependencies):
    # ... [Include the entire PERT function code here]

# Example usage
tasks = {
    "A": (3, 7, 5),
    "B": (2, 6, 4),
    # ... [Rest of your tasks]
}

dependencies = {
    "A": [],
    "B": [],
    # ... [Rest of your dependencies]
}

results = pert(tasks, dependencies)

#Print the results
results_df = pd.DataFrame.from_dict(results, orient='index')
print(results_df)
```

## 📄 Licencia

Este proyecto está bajo la licencia MIT - consulta el archivo [LICENSE](LICENSE) para más detalles.

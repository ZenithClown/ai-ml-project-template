<h1 align = "center">HOWTO</h1>

<div align = "justify">

The template provides a minimal approach for getting started with an AI/ML project, and has hardly any dependencies required. However, the [`notebooks/BOILERPLATE.ipynb`](notebooks/BOILERPLATE.ipynb) provides popular import and its configurations (like `pandas`, `numpy`, `scikit-learn` and `tensorflow`). A high level directory overview is as follows:

```
├───config          : store all configuration files
│
├───data            : responsible for all data handling, or contains raw data
│   └───processed   : contains processed data (like combined/normalized dataframes, tables, etc.)
│
├───logs            : repository to contain log files, can also be saved in `/path/to/directory`
│
├───notebooks       : contains boilerplate notebook for EDA and quick data understanding/explanations
│
├───output          : directory responsible for all output files
│   ├───images      : save output images
│   └───savedmodels : save trained model files
│
├───src             : source directory
│   ├───agents      : define agents for any rnn application
│   ├───engine      : provides a suit of machine learning analytic functions
│   └───models      : directory containing model definations
│
├───static          : other important/useful resources required in the project
│   ├───fonts       : store additional fonts, maybe used in documentations
│   ├───images      : store explanatory images
│   └───logo        : setup a project logo
│
└───utilities       : utilities directory containing functions and/or submodules
```

</div>

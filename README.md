# Johnson's simple data science project template

This template is based on the workflow description and project layout from [Data Science for Social Good](https://github.com/dssg/hitchhikers-guide/tree/master/sources/curriculum/0_before_you_start/pipelines-and-project-workflow). They clearly know what they are doing far more than me, but I wanted my own version to muck about with and adapt as I get better at these things.

One day I may even document this, but for now you'd be better off using someone else's template.  

`
├── data
│   ├── 01_raw
│   ├── 02_intermediate
│   ├── 03_processed
│   ├── 04_models
│   ├── 05_model_output
│   └── 06_reporting
├── docs
├── notebooks
│   └── 20000101-jc-notebook-template.ipynb
├── README.md
├── references
├── requirements.txt
├── results
└── src
    ├── d00_utils
    │   ├── my_fun.py
    ├── d01_data
    ├── d02_intermediate
    ├── d03_processing
    ├── d04_modelling
    ├── d05_evaluation
    ├── d06_reporting
    ├── d06_visualization
    └── __init__.py
`

There are README files in each empty folder to force git to add them to the repository.

Data in various stages of processing goes into the data directories.
Functions and source code goes into the `src` directory according to the required workflow step.
The `src` directory is a module - see how it's used in the notebook template. 
Distributable material should end up in the `results` directory, and any additional instructions and such in the `references` directory.
`docs` is used for Sphinx documentation, if I ever care enough to do that....
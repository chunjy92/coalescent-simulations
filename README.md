# Coalescent Simulations
Simulates different coalescents

## Dependencies

* Python 3.6
* Requirements:
  * biopython==1.68
  * matplotlib==2.0.0
  * numpy==1.12.0
  * scikit-learn==0.18.1
  * scipy==0.19.0

## Usage
Parameters can be customized. For available options:
```
python main.py -h
```

1. **Model Test**
    
    ```
    python main.py --test
    ```

* Produces a single tree for Kingman and Bolthausen-Sznitman
* Enable graphics output with `--graphics`
* Current default setting:
  * Sample Size: 10
  * Mutation Rate: 0.9
  * Number of Iterations: 300

2. **Experiment**
* Executes a number of Experiments and records experimental data for analysis 
* Current default setting:
    * Sample Size Range: (5, 10, 5)
    * Init Mutation Rate: 0.9
    * Mutation Rate Step: 0.3
    * Number of Process: 1
    * Number of Experiments: 3
    1. Single Process (with default params):
        ```
        python main.py
        ```
    2. Multiprocessing (with default params):
        ```
        python main.py --num_proc n
        ```
        wtih *n* number of processes

## Timeline
* First Implementation : 2015 ~ 2016 Academic year

* Current Status : March 2017 ~

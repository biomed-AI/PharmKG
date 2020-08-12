# PharmKG

The code for our paper: ***

The code was built based on pykeen (https://github.com/pykeen/pykeen). Thanks a lot for their code sharing!

## Overview

### (Result)

## Installation

Under the "PharmKG-D/model/pykeen/pykeen" directory, type `python setup.py install --user` to compile the pykeen package.

## Dataset

Run code `python PharmKG-D/data/preprocess.py`

## Baselines

### Pykeen

#### Model

`TransE`, `TransR`, `DistMult`, `ComplEx`, `RESCAL`

#### Training

Run code `python PharmKG-D/model/pykeen/train.py --model <model_name> --save_path <path>` under the root directory of this repository.  `<model_name>` is name of the model you are going to train. `<path>` is the path to a json file containing the output results.

### KBAT

#### Model

`ConvE`, `ConvKB`

#### ConvE

Run code `sh PharmKG-D/model/ConvE/run.sh`

#### ConvKB



### HRGAT



### Hyperparameter Optimization

We used default hyperparameters in package `pykeen`. If you want ***, please modify the hyperparameters in file `PharmK-D/model/pykeen/train.py`. 


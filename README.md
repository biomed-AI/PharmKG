# PharmKG

The code for the paper: PharmKG -- A Dedicated Knowledge Graph Benchmark for Biomedical Data Mining

The code was partly built based on [Pykeen](https://github.com/pykeen/pykeen) and [KG-reeval](https://github.com/svjan5/kg-reeval). Thanks a lot for their code sharing!

## Overview
PharmKG is a multi-relational, attributed biomedical knowledge graph, comsed of more than 500 thousands individual interconnectons between genes, drugs and diseases, with 29 relation types over a vocabulary of ~8000 disambiguated entites.

![PharmKG](pharmkg.jpg)
<!-- ### (Result) -->

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

### Neural network-based method

#### Model

`ConvE`, `ConvKB`, `RGCN`, `HRGAT`

#### ConvE

Run code `sh PharmKG-D/model/ConvE/run.sh`

#### ConvKB



#### RGCN

#### HRGAT

Please unzip the file `/PharmKG-D/data/PharmKG_origin.zip` and replace the file `PharmKG.csv` first

Run code `sh PharmKG-D/model/HRGAT/run.sh`

<!-- ### Hyperparameter Optimization

We used default hyperparameters in package `pykeen`. If you want to try , please modify the hyperparameters in file `PharmK-D/model/pykeen/train.py`.  -->


## Sponsor info
Initial development was supported by Aladdin Healthcare Tech and Sun Yat-sen University.


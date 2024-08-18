# Argument Pair Extraction
This repository hosts the code for the paper: [*Have my arguments been replied to? Argument Pair Extraction as Machine Reading Comprehension*](https://aclanthology.org/2022.acl-short.4/). 

The original code is available in [this repo](https://github.com/hlt-hitsz/mrc_ape), but I simplified it for students at the University of Indonesia to do their final project.

# Steps to Run

First, create a Conda environment---[resource to install Miniconda](https://docs.anaconda.com/miniconda/miniconda-install/)---with the following command:
```bash
conda create env 
```

# Prerequisites
python 3.7  
pytorch 1.8.0  
cuda 10.2  
transformers 2.11.0  

# Usage
python prepare.py  
python to_bioes.py  
python run.py  

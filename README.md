# Argument Pair Extraction
This repository hosts the code for the paper: [*Have my arguments been replied to? Argument Pair Extraction as Machine Reading Comprehension*](https://aclanthology.org/2022.acl-short.4/). 

The original code is available in [this repo](https://github.com/hlt-hitsz/mrc_ape), but I simplified it for the NLP students at the University of Indonesia to do their final project.

# Steps to Run Locally

First, create a Conda environment---[resource to install Miniconda](https://docs.anaconda.com/miniconda/miniconda-install/)---with the following command:
```bash
conda create -n ape python=3.10
conda activate ape
```

Second, install the requirements with the following command:
```bash
pip install -r requirements.txt
```

Third, run the scripts in `downloader.ipynb` in `data/` and `longformer-base/`
to download data and longformer model.

Fourth, create a folder in `data/` named `processed/`

Last, run the following command:
```bash
python prepare.py  
python to_bioes.py  
python run.py
```

Notice that there will be a new folder named `saved_models`, which consists of the trained model and a log file detailing the F1 score(s) for each epoch.

# Alternative

You may compile everything into a Jupyter Notebook file and run it through platforms such as Kaggle or Colab. By doing this, you can leverage free GPUs to accelerate the process.

# Data download

1. Download Data

* download by command (mac)
    ```shell script
    ./download.sh 
    ```

* download by link
    >   download and unzip under folder named 'data'
    >
    >   [data.zip](https://drive.google.com/uc?id=1Gs9Per_unwdmlXufDxmYEgLAve0ep8Xx)

2. Download trained models

    >   download and unzip models of the paper
    >
    >   [models_paper.zip](https://drive.google.com/uc?id=1wdf5UbkW4lV4RYQtMbKLmokN85PREIQI)
    >
    >   [models_paper_mean_std.zip](https://drive.google.com/uc?id=1It14qQhnawW7sXSwAZ94CMIYcgHp80SW)


# Conda Setting

```shell script
curl -O https://repo.anaconda.com/archive/Anaconda3-2019.10-Linux-x86_64.sh
sha256sum Anaconda3-2019.10-Linux-x86_64.sh
bash Anaconda3-2019.10-Linux-x86_64.sh

conda create -n maxwellfdfd-ai 
conda activate maxwellfdfd-ai
pip install -r requirements.txt 
```
optionally, use conda and conda-forge to install relevant packages
 
# Run script 

* Train
    - default
    ```shell script
    python train.py 
    ```
 
    - different model, loss function
    ```shell script
    python train.py -m rf -l diff_rmse
    ```


* Test
    ```shell script
    python test.py 
    python test_ensemble.py
    ```

* Evaluate single data

    ```shell script
    python evaluate.py 
    ```

## To generate the data please visit the following GitHub URL : 
https://github.com/wonderit/maxwellfdfd

## How to Cite
Kim, W., Seok, J. Simulation acceleration for transmittance of electromagnetic waves in 2D slit arrays using deep learning. Sci Rep 10, 10535 (2020). https://doi.org/10.1038/s41598-020-67545-x

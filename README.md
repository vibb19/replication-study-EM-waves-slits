# Data download

1. Download Data

* download by command (mac)
>   ```shell script
>   ./download.sh 
>   ```

* download by link
>   download and unzip under folder named 'data'
>   [data.zip](https://drive.google.com/uc?id=14-Bl89OzRtLM1MCW2H81Xvivq8EvTrmB)

2. Download trained models

>   download and unzip models of the paper
>   [models_paper.zip](https://drive.google.com/uc?id=1lvexOJmZ8zGHecwOwAGBoEjxRj9YXBO4)
>   [models_paper_mean_std.zip](https://drive.google.com/uc?id=1lvexOJmZ8zGHecwOwAGBoEjxRj9YXBO4)


# Conda Setting

```shell script
curl -O https://repo.anaconda.com/archive/Anaconda3-2019.10-Linux-x86_64.sh
sha256sum Anaconda3-2019.10-Linux-x86_64.sh
bash Anaconda3-2019.10-Linux-x86_64.sh

conda create -n maxwellfdfd-ai python=3.7
conda activate maxwellfdfd-ai
pip install -r requirements.txt
```

 
# Run script 

* Train
>   - default
>   ```shell script
>   python train.py 
>   ```
 
>   - different model, loss function
>   ```shell script
>   python train.py -m rf -l diff_rmse
>   ```


* Test
>   ```shell script
>   python test.py 
>   python test_ensemble.py
>   ```

* Evaluate single data

>   ```shell script
>   python evaluate.py 
>   ```
<details>
  <summary>Menu of ReadMe</summary>
  <ol>
    <li>
      <a href="#about-the-project">About The Project</a>
      <ul>
        <li><a href="#built-with">Built With</a></li>
      </ul>
    </li>
    <li>
      <a href="#getting-started">Getting Started</a>
      <ul>
        <li><a href="#prerequisites">Prerequisites</a></li>
        <li><a href="#installation">Installation</a></li>
        <ul>
        <li><a href="#step-1-set-environments">Step 1: Set environments</a></li>
        <li><a href="#step-2-set-dataset">Step 2: Set dataset</a></li> 
      </ul>
      </ul>
    </li>
    <li>
      <a href="#usage">Usage</a></li>
      <ul>
        <li><a href="#train">Train</a></li>
        <li><a href="#evaluation">Evaluation</a></li>
      </ul>
    <li><a href="#contributing">Contributing</a></li>
    <li><a href="#license">License</a></li>
    <li><a href="#contact">Contact</a></li>
    <li><a href="#acknowledgments">Acknowledgments</a></li>
  </ol>
</details>


# About The [Project](https://github.com/Cmput-414/PoinTr/blob/master/documentation.md)  
[Click Here to see ***Project Documentation***](https://github.com/Cmput-414/PoinTr/blob/master/documentation.md)  
[Click Here to see Original Author's README.md](https://github.com/Cmput-414/PoinTr/blob/master/README_old.md)  
**This project is 3D Point Cloud Inpainting.  
In this project, we add label to modify the loss function.  
We also change the DG-CNN to improve the F-score and CDL.**  

## Project Flowchart - Click image to see HD version and ZOOM IN/OUT  
[![Project Flow chart](https://kroki.io/mermaid/svg/eNqNVlGP2kYQfs-vGPnJnAjpwV0fkFqpB40U9ZpYwXkJF6HFrI0VY7vrdZKr-PH9ZnYNdghVeAB2d2Z25ptvZiczqt5TvHxB-PyxXlll7KeXL38n-hgGB5WXk_r5qaQ3lpK9Tj5TnlJe1i2W1eGgyh3lDWVVXmZkK7IGClQZsrqxE1aDtGURORmT3euSElUUZNpyU2objoZi0OtL8dqLBSNx8SOxcw9hAAOlNuJdvIdq_Wz3VUlpXmj4Vlr25HQJsaeXxh7Y2DFm344UR_09yGJrJVsv5Ltpt5kDK6J1IEocdmSqRDdN8EmEFutgp9PzxRwcwzUnZbJmzJ6leTZ2eGy-mtxqM6YvqvD_IX9zcyMBpW2Z2BwhAWaVaafCN9buxjE9lUBNcNq2ebETNACAaSxtdVoZTQ2n86zZOekwdDl_XMlqGQYr9UWT8nmukVPbwbQUkWMQc2KyirYKEsj3INSTw2PaVWQAYOdpcKSHVexMrWKx5Zd-FblV5FaPDnVd7oa4s-46ePhRZD6wXW60wyx-cJFOw-A1AzI-01cywWTrWJKXsHhQrAf41bYCu-F-e9CIJG-sybet1bsx1coAbF1ACkg0mr7mwP6gPveSk6oGaSSP3GIqES1mYfBeLPbRpTD5XNtRJzoT4qEU2L-Jc-CIbeguOMcCtuxuDtVOF-EVTUFmw6YlyrKy9LYqxdRdz1RRqd33hry3U6C2ED-X5_BfRT76k_B0cG0PKVx1F35oGI6eAVoqq04YXhhhP39g6L4zdKl8SZAlrR9OlXCFEsvbMDiXi6QSKA37xg6XNdpuvJzvHwLWeQ-qQ_4LG1z5SVFeWkHJyKI7ckTyve4782dhOegYtbwFXsntL67PXFwBiy2IaSuT7CetzQvgCZkJw_eIjIOasMu5F12IG21bU1KjDnXBvYi3C5H0ReVunPobL0HwBrZwxPFpoDfzeg2ay0bIL9wXTWk4TFRSliav9Ldam_ygS9sMTNx5E33GQpvD8dgMWj07siMknNn0VIoYp0-jy7ZS5dzk-Fb8O78JZz0-Gzhw7x0YVh9c8DXtzfW9QGtOT43G6XXdF1C6dsqleMTydu0I6V_assl32geWVsU5EZCUYun0ps4r0XVObVJTHTZJmrED711eFLMaFdUmXIOeMNTUOsnTHDvb5xOLSnXQ_q6L2pLeu_qpprtChTnJoqpq-rOukn0wcm0fnWWF61103cTA9c07nuIr14ZWs64LdU5DPsMPGpHNVUFhXmIIAWuth2s0B35_vYnjN_iNFm87e6f-CENsBynB6ZFW6IedMUbOv8q9CrhuQK6BifvvTAhPQDfkYWequkZs4Fbuk5o3CbIcXOlfEWMcoTxiQ3_3KukC4QgIO7mOMzJifHv-N_TOMDvftVa2k0oZ1KbU3SYpqhZPmdGONrLZjAu1PTX26Na9yZwqq2u6ndMHtJRogZGnbPiplDFlsGZEJHy8nRyp1IbQ759Wm-fxD3zobnPJjmb-tukcmq7vuUdyIDxzwndeeDan16gQYPxWd8NKdOdk7r3M3ZzSuukO793hr_7wft61L_zQb-HPQjWiaznEOLUOiqo5z2_XkviIJDJbQOkNK_SHRXgzpsyGmYELqF27H2FKhH5lwkRZnVXmuZ9i1t8458dukeZl93dRdOE_utQ-8vuOylGYowauSp-UotVctKQyfg0nk8m1aGOOlmfla0HGPshznz0Hedrrj8aj_5uAoQBBDL3yxmHVmzp9h4mn7l5Hq3h28ttP8vz5Dzj0HNA)](https://mermaid.live/view#pako:eNqNV9tu2zgQ_RVCT06hupEvSWpgF9jYu0Cx2a5Qqy-NC4OWKFuoLGopqq1b99_3DEld7LhBkweb5Mxw5syZ4fi7F8tEeDNvq3i5Y9FiVTD8_fG41Fzpjy9f_s7Yh8HK2_OsGJaHFY7faBbvRPyJZSnLirLGUu73vEhYVrGtzIot05JpBQ0mFdOi0kOjB3FNMubIZ3onChbzPGeqLtaF0IOrMzlo9sVo3ch5V9bRD4xcvIeHMFIIZX2MdlAvD3onC5ZmuYCHhSZ_2psY-XvJ4D0ZPEbk4pFF4ckmxLG3tHurwn5W9cZhF7LHlWc0CYNQyVhU1cr7aOXmOExE2rlgYiX8ZoyrbeWTk2m29S0-6y8q00L57DPP3XdSePHihQkurYtYZwgPwPOtsDp0bWmv9RmkAaMBblNneWKwARqq0mwjUqkEqyjHnWrnqgXVceFhaZYLYLzknwXjLv0lUq073BZG6ggEKGFbyTYcQmDCSdCt4z5LJFNAtPF45R3Z_TJy1paRMdes3TJ0y9AuH1wqRJGc5YL0gff9pTjbMJNMCQtidO8CHyHIvwgiv-O4yQ7xsSFRVsDqnpMmpYRvJGoAodR7gaiySqtsU2uR-KzkCviLnMQASyXYlwz52PNPvYylvEJyWYvkfGSCm4_hyztjtQ84G8SfSn3VSY8NN1E05ObQunHENqnPKfsGf7O93qPW88FPlQ1Oa7Jv4i2kZm9lYaxN-tZyyZOntpzbI8JwbhxedFi8ChsoOvnRyeU94HDhZPC-InB6JtiCa95C-tQKuXvB0rSxdEH7AnEW7PG-LZefEmURIMiurGx-Adlpt0lwZSX02gm6rmOA6_ZI97REDEdsoZryfWoGVWUWzZHjl-uTZxd00uagI9oiAHJxcO0a05NryGoNzmqp4t2w1lkObCE0JCgfwAGwFraJDUaZ5JXQtSpYxfdlTt2L9nMj2padvXbUXHsBDmdkA3cszc50x41uhX60NsVhasNqmyZFJGZcs-Er8bUUKtuLQldnZiaNmRM-Q4Jic2CdvBnkUMJAA6IZBI0cpVSgSdemIVB3pKvxrXtdOkU6O_Ni2nhxVqOQcdXvTPZdoeaeto3Janb9G-DaZkwVe8QyeHRsbZ7wosoS4UJMZd5PD6RNRTW6I-ee0bferVMl9-s43RpH3tlscaI9Cq-OqVYdmVhVijhLM-xsDi3DCr4X7X1Pa9D27uWvNu0l1aKVzqUs2Z-ljHcguX1AqBst4YiNtRlMqCHQTlsLS9u9luO2eTURQGWLD_QvnfGcDbIC4w7IrR1-VzNC9O83UfSGvoTzt53Rtr3CGNlCrnB-ZEtqp41FAtO9-f1qecaGuQxWpudWDI1ASGQnUbIsESbYl7lsZ1VM-fd-2vxCA3yIUooU--ek8J7CHhLsVrZllRlmvh6-DZxXhsX_1trsx5IrFLSp1HWcyxoPpBKWVmaz8nO-6b0QYWAffZNCLUoWzNh79KNwjiGrqOgRtkPRyQYBZMDAq0xx20IyFP2vFurgX3Cku9LSIBw3V45mULbd0z6_Z_JjKz9p5Mcz9hfqCcC_Fd1wFE6s2LQRm8xYWlbd-dSe3zTn01nTBPHBfhv8KnZX7Jn0YpBDenNZdePjM_l9oPwSocD-NSmdTKxwy2dbPdgq-IKi17srjKowIdUg5lpspTqcZJ8srG0Yvl2kWdF8necdFg826w9mjEClcQxwJz6bjmsqXVClM76lt3Y4HD4TemRCpwH-mYijJuKuc_cibjf7w_rVszM5NCCJKdy8olj15t-mQUUjd7llXjTuhdD90Gj-Pd8DxfFjLMFPtu90vvLwA4na6YwZ53mdI8ZV8QOivNZyeShib4YMCd-rS_QQscg4QNk3myUvvNl376s3m1wPryfTyTQIxnfTSXA79b2DN3t5GwxvR-NxcBdMpq9fX49--N43KaE_Gl7fXt_djKbj4OYmeH13OzbWPphDMv7jf_lbrek)
## Built With
* [![Python][Python.com]][Python-url]
* [![Pytorch][Pytorch.com]][Pytorch-url]
* [![Cuda][Cuda.com]][Cuda-url]


# Getting Started
There are two ways to set environments. We **recommend** to use Colab without output.  
- First is using:
  - [**colab without output**](https://github.com/Cmput-414/PoinTr/blob/master/Project%20Implementation.ipynb).  
  - [**colab with output**](https://github.com/Cmput-414/PoinTr/blob/master/project_implementation_with_output.ipynb).  
- Second is follow the below instructions.  

## Prerequisites 
- python==3.6 

- pytorch==1.4.0  

- torchvision==0.5.0

- cudatoolkit=10.0  

- GCC>= 4.9


## Installation  

### Step 1: Set environments  (~20 minutes)

1. Git clone the code
    ```
    git clone https://github.com/Cmput-414/PoinTr.git pointr
    ```
2. Install the code to create a virtual environment
    ```
    wget https://repo.anaconda.com/miniconda/Miniconda3-py37_4.12.0-Linux-x86_64.sh
    chmod +x Miniconda3-py37_4.12.0-Linux-x86_64.sh
    bash ./Miniconda3-py37_4.12.0-Linux-x86_64.sh -b -f -p /usr/local/
    conda create --no-default-packages -n myenv python=3.6 --yes
    ``` 
3. Activate environment and install packages  
    ```
    source activate myenv && which python && conda install pytorch==1.4.0 torchvision==0.5.0 cudatoolkit=10.0 -c pytorch -y
    source activate myenv && pip install ninja
    source activate myenv && git config --global url."https://".insteadOf git://
    source activate myenv && pip install "git+git://github.com/erikwijmans/Pointnet2_PyTorch.git#egg=pointnet2_ops&subdirectory=pointnet2_ops_lib"
    source activate myenv && pip install --upgrade https://github.com/unlimblue/KNN_CUDA/releases/download/0.1/KNN_CUDA-0.1-py3-none-any.whl

    ``` 
4. install requirments and some modules
    ```
    source activate myenv && pip install -r requirements.txt
    source activate myenv && cd /content/pointr/extensions/chamfer_dist && python setup.py install --user
    source activate myenv && cd /content/pointr/extensions/cubic_feature_sampling && python setup.py install --user
    source activate myenv && cd /content/pointr/extensions/gridding && python setup.py install --user 
    source activate myenv && cd /content/pointr/extensions/gridding_loss && python setup.py install --user
    ```
### Step 2: Set dataset   (~15 minutes)
There are 2 ways to set dataset, we **recommend** to use frist method:  
- **First method**:  
 We aleady shared a google drive folder [`Pointr`] to guanfang@ualberta.ca and basu@ualberta.ca. This folder contain the dataset.  
 After you access the shared folder, you can run below code to set dataset.  
  1. First connect to your google drive to access shared drive
        ```
        from google.colab import drive
        drive.mount('/content/drive')
        ```
  2. Then run rest code to set dataset  
  *sometimes Colab use gdrive as google drive folder-
  ex: /content/**g**drive/Shareddrives
      1. set KITTI dataset
            ```
            cp -r '/content/drive/Shareddrives/Pointr/kitti/bboxes' /content/pointr/data/KITTI
            cp -r '/content/drive/Shareddrives/Pointr/kitti/cars' /content/pointr/data/KITTI
            cp -r '/content/drive/Shareddrives/Pointr/kitti/tracklets' /content/pointr/data/KITTI
            ```
      2. Set ShapeNetCompletion (PCN) dataset  
            ```
            unzip /content/drive/Shareddrives/Pointr/PCN.zip -d /
            ```
- **Second method**:  
You will need to dowload them or add them to your google drive.  
Follow the data structure in [new_data.md](./new_data.md).  
Make sure set the data into correct location.   

    | dataset  | url |
    | --- | --- |
    | PCN |   [[Google Drive](https://drive.google.com/file/d/1hHIoAW97HUsc2A9F159xutd0ajar1mqi/view?usp=share_link)] |
    | KITTI | [[Google Drive](https://drive.google.com/drive/folders/1fSu0_huWhticAlzLh3Ejpg8zxzqO1z-F?usp=share_link)]  | 

# Usage  

## Train  

We will first to train the model to get F-score, CDL1, CDL2, and save the result as check point.  
The we will use best check point to do test with some visual result (images).   

0. Basic format for train
    ```
    bash ./scripts/train.sh <GPUIDS>
        --config <config>
        --exp_name <name> 
    ```
1. Train Pointr model on KITTI dataset with 1 GPU
    ```
    cd /content/pointr
    source activate myenv && which python && bash ./scripts/train.sh 0 --config ./cfgs/KITTI_models/PoinTr.yaml --exp_name example 
    ```
2. Train Pointr model on PCN dataset with 1 GPU 
    ```
    cd /content/pointr
    source activate myenv && which python && bash ./scripts/train.sh 0 --config ./cfgs/PCN_models/PoinTr.yaml --exp_name example 
    ```

## Evaluation   
### Do test from Pretrain model
Instead start trsing to do test, we also have some pretrain model.
| Pretrained model | Download LInk |  
| --- | --- |  
| KITTI | [[Google Drive](https://drive.google.com/drive/folders/1XHxak8eOQBTqrPJL7dXQipLajWiSOKQh?usp=share_link)]|  
| PCN | [[Google Drive](https://drive.google.com/file/d/1-L2bqK2dRMjSkDR8K6LEe_ad6JFT3kwj/view?usp=share_link)] |  

Download pretrained model into ./pretrained folder  
```
mkdir pretrained
cp -r /content/drive/Shareddrives/Pointr/pretrain/kitti-ckpt-best.pth -d /content/pointr/pretrained
cp -r /content/drive/Shareddrives/Pointr/pretrain/pcn-ckpt_best.pth -d /content/pointr/pretrained  
```  
***For example: load pretrained model for KITTI***  
/content/pointr/pretrained/kitti-ckpt-best.pth  
***For example: load pretrained model for PCN***  
/content/pointr/pretrained/pcn-ckpt-best.pth  
```
source activate myenv && which python && bash ./scripts/test.sh 0 --ckpts ./pretrained/kitti-ckpt-best.pth --config ./cfgs/KITTI_models/PoinTr.yaml --exp_name example
```  

### Do test from new training
we will use result from training to do evaluation.  
The training result will save into ./experiments/PoinTr  
We will use the best check point (ckpt_best.pth) to do evaluation.  
After test, we will be able to see some visual result (images) in folder ./vis_result.

0. Basic format for test
    ```
    bash ./scripts/test.sh <GPU_IDS>  \
        --ckpts <path> \
        --config <config> \
        --exp_name <name> \
        [--mode <easy/median/hard>]
    ```
1. Test PoinTr trained model on KITTI dataset:
    ```
    cd /content/pointr
    source activate myenv && which python && bash ./scripts/test.sh 0 --ckpts ./experiments/PoinTr/KITTI_models/example/ckpt-best.pth --config ./cfgs/KITTI_models/PoinTr.yaml --exp_name example
    ```  
2. Test PoinTr trained model on PCN dataset:
    ```
    cd /content/pointr
    source activate myenv && which python && bash ./scripts/test.sh 0 --ckpts ./experiments/PoinTr/PCN_models/example/ckpt-best.pth --config ./cfgs/PCN_models/PoinTr.yaml --exp_name example
    ```


# Contributing

What we do:  
1. Add 3D CNN, we call it LBCNN
2. Add label to modify the lose function.  
2. Change the DG-CNN to improve the F-score and CDL.
3. Draw a flowchart for project
4. Write a documentation for code.
5. Set a environment in colab

- A visual result on KITTI datset.  
  - 10 epoch, 16 batch size

[![Watch the video](https://github.com/Cmput-414/PoinTr/blob/master/fig/image.png)](https://www.youtube.com/watch?v=NMUYv3yEMac) 

# License

Distributed under the MIT License. 



# Contact

| Name | Email |  
| --- | --- |  
| Shiqi Zhang | shiqi@ualberta.ca |  
| Peng Cheng | pcheng1@ualberta.ca |  


# Acknowledgments

* [Paper & Base code - Pointr](https://github.com/yuxumin/PoinTr) -  [Xumin Yu](https://yuxumin.github.io/)\*, [Yongming Rao](https://raoyongming.github.io/)\*, [Ziyi Wang](https://github.com/LavenderLA), [Zuyan Liu](https://github.com/lzy-19), [Jiwen Lu](https://scholar.google.com/citations?user=TN8uDQoAAAAJ&hl=en&authuser=1), [Jie Zhou](https://scholar.google.com/citations?user=6a79aPwAAAAJ&hl=en&authuser=1)    
* [ReadMe file format](https://github.com/othneildrew/Best-README-Template)


[Python.com]: https://img.shields.io/badge/python%203.6-ffffff?logo=python
[Python-url]: https://python.com 
[Pytorch.com]: https://img.shields.io/badge/pytorch%201.4-FFFFFF?logo=pytorch
[Pytorch-url]: https://Pytorch.com
[Cuda.com]: https://img.shields.io/badge/cuda%20%2010.0%20-FFFFFF?logo=nvidia
[Cuda-url]: https://developer.nvidia.com/cuda-10.0-download-archive

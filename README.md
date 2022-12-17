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
In this project, we add label to modify the lose function.  
We also change the DG-CNN to improve the F-score and CDL.**  

## Project Flowchart - Click image to see HD version and ZOOM IN/OUT  
[![Project Flow chart](https://kroki.io/mermaid/svg/eNqNV1Fv2zYQfu-vOOjJLlx3sZM-GNiAxV6BYF4m1OpL08KgZUoWKosaRbXN4B-_746ULdf10DwkJn13_O67745MblW9o2TxgvDz-9PKKes-vXr1G9GHQbRXRTWunz9W9OAo3en0MxUZFVXdYmn2e1VtqWgoN0WVkzPkLBzIWHK6cWN2g7VjE_lmRG6nK0pVWZJtq3Wl3WB4bga_vhWvg1k0FIgfiMHdDyIEqLQVdMkOrvWz25mKsqLUwFY5RnI8hBjpZbB7DnZIGNuBkri_B1tsrWTrhfxu2k3uyYrpKRInTju2JtVNE30So_lTtNXZ6WBOjumakbJ5M2JkWZGPPB_rr7Zw2o7oiyrDZ9i_fPlSEsraKnUFUgLNKtfehU-s_Ykj-liBNeFp0xblVtgAAbZxtNGZsZoaLufJswPpOfQ1X65ktRhEK_VFkwp1rlFT19G0EJNDlHBhckMbBQvU-yzVI-ARbQ1ZENghjQ50v0p8qFUiscIyrGK_iv1q6VnX1facd_Z9iu5_lFlIbFtY7TlL7n2mk0H0lgkZneQrlWCxdSopKkTcK_YD_WpjoG7Ab_camRSNs8WmdXo7olpZkK1LWIGJRtPXAtzv1edecTLVoIwUmJtPJKP5dBC9k4h9dmmQfq7dsDOdivDQCoxv7AEcsA3fOddYyJbd9d5sdTm44inMrDm0ZFkZR4-mklC3vVClUdvvAwW0E7A2F5yLU_qv45D90XhydmyPKRx1O3jfMB29ALRQTh05vAjCOH8Q6K4LdOl8KZAFPd0fO-GKJBY3g-jULlJKsHQ-N7Y4rNFuHezC_BCyTntwPde_qMG3nzTlZRS0jCy6r7yQwqz7LvzJWL7oFLW4AV_pzS9-zlwcgYgthOmMTXfj1hUl-ITNmOlbouKQJuJy7cUX5la71lbUqH1d8izi7VIsQ1P5EyfhxEsSQoANgHg9nflNg1-D4bIW8Yv2xVMGDguVlKPxa_2t1rbY68o1ZyFuQ4i-YuHN6QRuzkY9A9kSCs5q-liJGZdPY8q20uU85PhUfDrdCSc__u4MwF0AcN59gBB6OoTro8Bozo6Dxvt10xdU-nHKrXjA8ubJCzLctFVTbHVILDPlqRCwlGbp_CYelfh6UOvMmv06zXIG8M7XRbGq0VFtyj0YBENNrdMiK7CzeT6qqFJ7Hc666C2ZvaufGrordJi3LI2p6Y_apLto6Mc-JssKx_vsuhcD9zfvBImv_BhaTbsp1IGGfY4_GESuUCUNigqPEKjWBbqGM_D350OSPOBvPH_s4h3nIwJxHJQE3x5ohXnYBWPmwq3c64DrAeQYhLj7LoToBHJDHbbW1DVyg7aKUNSiSVHl6Mr8ipnjGO2RWPqr10kXDMdg2Nt1mpEnxrfnfwcBDKvz79bJdmqURW9K363T0rS4yqz2spHNZlSqzXGwxzf-TuZSOV3TzYzeY6TEczx5qoavSnmmnK2ZEUkfdydnKr0h8vun1fZ59AMM3Wm-2PE0nDaZwdPPPX9JijHizc1-U1SK8tJs8FzKtEJ8LZ0tZ8iny2PwvHzo3qvsLzRCSJX-hi7Aid1bMJ56ILcByHRGb9F9qN8jD-oOFNqpbOWK77-Q4tvgfBe8b2e0vJ8_PjJwC6iahGI0tO24p5DCEcDtnQ_SxbibUVZjgi3M18qPZ34Z92npPIPjm-D4ZtYNZfyhXwc_K4AhXVMmHolP0dJABt0j75o0l5Am9wAadV2apuk_gYFmRLkb5BYQMJHcboi3L_yNHaTgKDf2uS9c9l978CO_yIqq-zgvm4B26QW75FcL5oGCKso-VFGGjCLNo4hUznf8eDy-lm3C2fJ_ANeSTEKSp9vjlORxr__gH_7fux4OMMRTXm5urHpv6TA3k4k_1zdLMj3iDv-f8M9_belnvg)](https://mermaid.live/view#pako:eNqNV11v2kgU_SsjP5HKpcEGUiHtShvYlapls6jQl4YKDWYMVo3HOx63oU3_-557x1-QNGrygGd8P8899874uxfpnfIm3t7I_CBWs3Um8PfH_dJKYz-9fv27EB97a-8ok6yfn9Z4_c6K6KCizyKJRZLlJZb6eJTZTiSF2Osk2wurhTXQENoIqwrbZz2IW5LhV76wB5WJSKapMGW2yZTtXV3IQbMrRutazrtygX4UFOItIoSRTBkX4-oA9fxkDzoTcZIqRJhZiqfxJCje5wzeksHHFYX4KFaLs02IY2_p9taZ-y3KbYXdQtyvPdYkDBZGR6oo1t4nJzfFy52K2xA4V8JvIqTZFz4FGSd73-Gz-WoSq4wvvsi0eiaFV69ecXJxmUU2QXoAXu6V0yG3uXPrC0gDRgZuWybpjrEBGqawYqtibZQoqMatahuqA7XiwnzJyxkwXsovSsiq_DlKbVvcZiz1CASoYHstthJCYMJZ0k3gvthpYYBoHfHaexS3y1Vlbblic_W6Wi6q5cIt51UpVLa7qAXpA-_b5_Js0twlRjkQV7dV4gGS_Isg8luOc3WIjzWJkgxWj5I0qSRyq9EDSKU8KmSVFNYk29KqnS9yaYC_SkkMsBRKfE1Qj6P83KlYLAsUVzRITgNObhoilvdstQu46EWfc3vVSofMTTQNhdl3YTxim9SnVH3Gn7c3R_R62vupMuO0Ifucb6atuNMZWxt2raVa7p7aqsIOCMMpBzxrsXizqKFo5YMz5x3g4HDY-1AQOB0TYiatbCB9aoXCfcbSqLb0jPYzxJmJ-9umXX5KlNkASbZt5eoLyM6nzQ4uC2U3lWA1dRi4do90z1uEOeIaldv3qRl0FS_qVxW_qjl54aCV5hct0WYDIBcNrqvB9MQNWS3BWatNdOiXNkmBLYT6BOUcHABrYZvYwMokb5QtTSYKecxTml60n7Jo03bObVC7fQaOysgW4TiaXeiGtW6BebTh5uDecNo8pIjEQlrRf6MecmWSo8pscWFmWJs54zMkKLcKrLMzgwLaCdCAaAZBlqOSKgzpkgcCTUdyjaf2dGkV6d1FFKM6iosehUzV_ZXJbig03ONmMDnNdn4DXDeMqWMfsRzcV2ytj_CsSHaqSjHWabc8kOaOqnWDKjzWd9FtYqOPmyjecyDvXbUk0R6NV0bUqxWZRJGrKIkT7GxPDcMyeVSNv6c96Gb38leH9pJ60UmnWufiz1xHB5DcHSA0jZYIxOVaX0xoINBO0wtLN72WYTO86gygsscP5pdNZCp6SYbrDshtK_yuJoTo3-9Wq3f0sJjetUab8QpjZAu1wvtHsaRxWlskMKszv9stL9hgZ7AyurTCNAIhUZ2d0XmONMG-pKp2UkRUf--nw2_BwC_QSisj_jlrvKewLwh2J9uwii8zD6dvvSoqZvG_peX9SEuDhuZO3USpLnFAGuVoxZuFn8pt54RYDNyhzyW0KheDifiAebSY4pKVFXQIu0vR2QYBxGDgVKa8XSMxRf8rlTn5zwTSunQ0WIS1y2ACZTc93fHr5CE91cdtkkmxT_UWV7RYSfhQPA7YDz89dUVX3Hf1rZkMMKggWaYe0C7w2d5FF6GLZlhHE07EX-hWlPWOh34dGnovLfkWcX4pWwwrA6PawnAi5rfTuzvOwCBmJRh0TAFTV0NUuXQCGY6cocbOaCLinGbgTH_N3LSnm_oZSI12pTyulceTesTjR_zW-1VmXIkXyItrKsg71yBIfcd8gb1zYi-1C3p7k-qiOLuPIyxf7G1vbxALRpo9XOEiDhPa9CJgttfmdMZtsrBxafhuESdZ_ThNiybuueP0nC9JmCMSlEm7MTNteI4pmmNC7ukm0e_3X0h9xanT58kLGa_qjNtzqZNxs9n9FLl68YsDGpDENwbfEbDq3O7r8bsKKueur1ZhJ4X2M6r-93wPDYxPzR0-SL_T-7UHUtFhMREcvCxT5LjOfkBUllYvT1nkTVAh5XtljgmpZokEKMd6M5eZN_nuPXiT1-PhTf96fBO8DYbB9XX4NvS9E7aD4dtBfzwYD7AXhOEwDH_43jetYWLYH4fXwU0QjK8Ho5vRdcj2PvI7Mv_jfwYn_Fw)
## Built With
* [![Python][Python.com]][Python-url]
* [![Pytorch][Pytorch.com]][Pytorch-url]
* [![Cuda][Cuda.com]][Cuda-url]


# Getting Started
There are two ways to set environments. We **recommend** to use Colab.  
- First is using [**colab**](https://github.com/Cmput-414/PoinTr/blob/master/Project%20Implementation.ipynb).  
- Second is follow the below instructions.  

## Prerequisites 
- python==3.6 

- pytorch==1.4.0  

- torchvision==0.5.0

- cudatoolkit=10.0  

- GCC>= 4.9


## Installation  

### Step 1: Set environments  (~14 minutes)

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
### Step 2: Set dataset   (~7 minutes)
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
  [![KITTI training](https://drive.google.com/drive/u/0/folders/0AMEcwIBVSoNtUk9PVA)](https://drive.google.com/file/d/1-I4xQdq0E747-h8XOQjhbCR5DCFpWmeZ/view?usp=share_link）




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

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


# About The [Project](https://github.com/Cmput-414/PoinTr)  

[Click Here to see Original Author's README.md](https://github.com/Cmput-414/PoinTr/blob/master/README_old.md)  
This project is 3D Point Cloud Inpainting.  
In this project, we add label to modify the lose function.  
We also change the DG-CNN to improve the F-score and CDL.  

## *** DIAGRAM NOT FINISHED***  
## Project Flowchart - Click image to see HD version and ZOOM IN/OUT  
[![Project Flow chart](https://kroki.io/mermaid/svg/eNqNVtGu2kYQfc9XjPxkIkJ64d4-ILVSLzRSVJpYwXkJidBi1saKsd31Osmt-PiemV2DHUIVHoDdnZmdOXNmdjKj6gPFy2eEzx-btVXGfnrx4neiD2FwVHk5qZ8-lvTaUnLQyWfKU8rLusWyOh5Vuae8oazKy4xsRdZAgSpDVjd2wmqQtiwiJ2OyB11SooqCTFtuS23D0VAMen0pXnuxYCQufiB27jEMYKDURryLD1Ctn-yhKinNCw3fSsuenC8h9vTa2CMbO8Xs24niqL8HWWytZeuZfDftLnNgRbQJRInDjkyV6KYJPonQYhPsdXq5mINjuOakTNaM2bM0z8YOj-1Xk1ttxvRFFf4_5J8_fy4BpW2Z2BwhAWaVaafCN9buxjF9LIGa4LRr82IvaAAA01ja6bQymhpO50Wzc9Jh6HK-WstqGQZr9UWT8nmukVPbwbQUkVMQc2KyinYKEsj3INSzw2PaV2QAYOdpcKLHdexMrWOx5Zd-FblV5FYrh7ou90PcWXcTPP4oMh_YPjfaYRY_ukinYfCKARlf6CuZYLJ1LMlLWDwq1gP8aleB3XC_PWpEkjfW5LvW6v2YamUAti4gBSQaTV9zYH9Un3vJSVWDNJJHbjGViBazMHgnFvvoUph8ru2oE50J8VAK7N_EOXDCNnQXnGMBW3a3x2qvi_CGpiCzZdMSZVlZelOVYuq-Z6qo1P57Q97bKVBbiJ_LS_gvIx_9WXg6uLaHFK66D983DEfPAC2VVWcMr4ywnz8w9NAZula-JsiSNo_nSrhBieVdGFzKRVIJlIZ9Y4_LGm23Xs73DwHrsgfVIf-FDa78pCivraBkZNEdOSL5Xved-YuwHHSMWt4Br-TuF9dnrq6AxRbEtJVJDpPW5gXwhMyE4Vsh46Am7HLuRRfiRtvWlNSoY11wL-LtQiR9Ubkbp_7GaxC8gR0ccXwa6M28XoPmshXyC_dFUxoOE5WUpclL_a3WJj_q0jYDE_feRJ-x0OZwPDaDVs-O7AkJZzZ9LEWM06fRZVupcm5yfCv-Xd6Eix6fDRx48A4Mqw8u-Jr25vpeoDWn50bj9LruCyhdO-VSPGF5t3GE9C9t2eR77QNLq-KSCEhKsXR6U-eV6DqntqmpjtskzdiBdy4vilmNimoTrkFPGGpqneRpjp3d05lFpTpqf9dVbUnvXf9U012jwpxkUVU1_VlXySEYubaPzrLG9S66bmLg-uYdT_G1a0PrWdeFOqchn-EHjcjmqqAwLzGEgLXWwzWaA7-_Xsfxa_xGizedvXN_hCG2g5Tg9ERr9MPOGCPnX-VeBdw2INfAxMN3JoQnoBvysDdVXSM2cCv3Sc2bBFkObvSviDGOUB6xob97lXSFcASEnVzHGRkxvj39G3pnmJ1vWyvbSaUMalPqbpsUVYunzGhHG9lsxoXanRt7dOfeZE6V1TXdzek9Wkq0wMhTNvxUypgyWDMiEj7eTo5UakPo90-rzdP4Bz50t7lkRzN_23QOTdf33CM5EJ454XsvPJvTK1QIMH6ju2EluncyD17mfk5p3XSHD-7wV3_4MO_aF37ot_BnoRrRrRxinNoEqwqAdePQrSSukERmCyi9Laqm6Q-L8GZMmQ0zAxdQu_YwwpQI_cqEibI6q8xTP8Wsv3XOj90izcvu76Lowl-51K74fUflKMxRRd9V6ZNStJqLllTGr-FkMrkVbczR8qx8K8jYB3nps5cgz3v90Xj0fxMwFCCIoVfeOKx6U6fvMPHU3etoFc_OfvtJnj__AeFPHJQ)](https://mermaid.live/view#pako:eNqNV22P2jgQ_itWPkGVoxCgyyLdSbdwlarjelFJv3SpkEkciBrinOO0paX__Z6x8wZLV939ALZnxjPPPDMevjuhjIQzd_aK5wcWLDcZw9-fj2vNlf74229_MPaht3GOPMkG-WmD4zeahQcRfmJJzJIsL7GUxyPPIpYUbC-TbM-0ZFpBg0nFtCj0wOhBXJOMOXKZPoiMhTxNmSqzbSZ0r38lB82uGK1rOadvHf3AyMUHeAgjmVDWx-AA9fykDzJjcZIKeJhp8qe5iZG_tww-kMFzQC6eWeBfbEIce2u7t8nsZ1HuKux89rhxjCZh4CsZiqLYOB-t3AKHkYhbF0yshN-ccbUvXHIyTvauxWf7RSVaKJd95mn1nRRevHhhgovLLNQJwgPwfC-sDl2b22tdBmnAaIDblUkaGWyAhio024lYKsEKynGr2rpqQa24sFqb5RIYr_lnwXiV_hyp1i1uSyN1BgKUsL1kOw4hMOEi6MZxl0WSKSBae7xxzuxhHVTW1oExV6-rpV8tfbtcVakQWXSVC9IH3g-34mzCjBIlLIjBQxW4hyBfE0Ruy3GTHeJjTaIkg9UjJ01KCd9J1ABCKY8CUSWFVsmu1CJyWc4V8BcpiQGWQrAvCfJx5J86GYt5geSyBsmFZ4JbjOHLO2O1CzjrhZ9y3W-lx4abKBpyc2DdOGOb1BeUfYO_2d4eUetp76fKBqct2TfxZlKztzIz1iZda6nk0VNbldseYbgwDi9bLF76NRStvHdxeQc4XDjpvS8InI4JtuSaN5A-tULu3rA0rS3d0L5BnCV7fGjK5adEWY4QZFtWNr-A7LLbRLiyEHpbCVZdxwDX7pHuZYkYjthCNeX71Ayqyizqo4pfVZ-8uqCVNgct0ZYjIBeOhlVjenINWS3BWS1VeBiUOkmBLYQGBOUKHABrYZvYYJRJXgldqowV_Jin1L1oPzWiTdnZa7362htwVEZ2cMfS7Ep3XOsW6EdbUxymNqy2aVJEYsY1G7wUX3OhkqPIdHFlZlKbueAzJCi2CqyLN4McihhoQDSDoJGjlAo06dI0BOqOdDW-ta9Lq0hnV15May-uahQyVfVXJruuUHOPm8ZkNdv-DXBtM6aKPWM5eqzYWj_hWZFEogoxlmk3PZA2FVXrepV7Rt96t42VPG7DeG8ceWezxYn2KLwypFqtyMSKXIRJnGBnd2oYlvGjaO57WoO2d69_tWmvqRatdCplzv7KZXgAye0DQt1oDUdsrPVgQg2BdppaWNvutR43zauOACp7fKB_6YSnrJdkGHdAbl3h158Ton-_CYI39MVfvG2NNu0VxsgWcoXzM1tTO60tEpjVm9-tlmdsmMtgZXptxdAIhER2IiXzHGGCfUmV7aQIKf_OT5ufb4D3UUqBYv9cFN5T2H2C3co2rDLDzNfTt17llWHxv6U2-6HkCgVtKnUbprLEA6mEpZXZLNyU7zovhD-yj75JoRY5G83Ze_Qjf4EhKyvoEbZD0cUGAWTAwKtMcdtCMhT9rxTq5N5wpL3S0sAf11d6cyjb7mmf3yv5sZWf1PLjOXuNegLwb0U7HPkTKzatxSZzFudFez6156_q8-m8boL4YL_3fhW7PnsmvRjkkN6VBIT1FPZMfleUXyIU2L9NZVFcTKxwy2V73dsr-IKi14c-RlWYkKoXci32Up0usk8WtjYM1y7iJKu_LtIWi5XN-sqMEag0jgEu7fpsOq6pdEGVzvie3trBYPBM6IEJnQb4ZyIO6ojbzt2JuNnsDuv9Z2dyaEASU7h5RbHqzL91gwq86nLLvGDcCaH9oVH_O64DiuPHWISfbN_pfOPgBxK10zkzzvMyRYyb7AdEeanl-pSFzhwZEq5T5ughYplwgHKsN3OeOfPvzldnPvJmg_vpaDYdeqNX4ztvPHOdE7ang9ndzLufeXf3w_u76d3sh-t8kxIWvMFsNB1CfjYcTr3JcGTMfTBnZP3H_yRFrfc)
## Built With
* [![Python][Python.com]][Python-url]
* [![Pytorch][Pytorch.com]][Pytorch-url]
* [![Cuda][Cuda.com]][Cuda-url]


# Getting Started
There are two ways to set environments. We **recommend** to use Colab.  
- First is using [**colab**](https://github.com/Cmput-414/PoinTr/blob/master/Project%20Implementation2.ipynb).  
- Second is follow the below instructions.  

## Prerequisites 
- python==3.6 

- pytorch==1.4.0  

- torchvision==0.5.0

- cudatoolkit=10.0  

- GCC>= 4.9


## Installation  

### Step 1: Set environments  

1. Git clone the code
    ```
    git clone https://github.com/Cmput-414/PoinTr.git
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
### Step 2: Set dataset  
There are 2 ways to set dataset, we **recommend** to use frist method:  
- **First method**:  
 We aleady shared a google drive folder to guanfang@ualberta.ca and basu@ualberta.ca. This folder contain the dataset.  
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
            unzip /content/drive/Shareddrives/Pointr/ShapeNetCompletion.zip -d /content/pointr/data
            cp -r '/content/pointr/data/PCN/PCN.json' /content/pointr/data/ShapeNetCompletion
            cp -r '/content/pointr/data/PCN/category.txt' /content/pointr/data/ShapeNetCompletion
            rm -rf /content/pointr/data/PCN
            mv /content/pointr/data/ShapeNetCompletion /content/pointr/data/PCN
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

we will use result from training to do evaluation.  
The training result wil save into ./experiments/PoinTr  
We will use the best check point (ckpts) to do evaluation.  
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







# License

Distributed under the MIT License. 



# Contact

| Name | Email |  
| --- | --- |  
| Shiqi Zhang | shiqi@ualberta.ca |  
| Peng Cheng | pcheng1@ualberta.ca |  


# Acknowledgments

* [Base code - Pointr](https://github.com/yuxumin/PoinTr)
* [ReadMe file format](https://github.com/othneildrew/Best-README-Template)


[Python.com]: https://img.shields.io/badge/python%203.6-ffffff?logo=python
[Python-url]: https://python.com 
[Pytorch.com]: https://img.shields.io/badge/pytorch%201.4-FFFFFF?logo=pytorch
[Pytorch-url]: https://Pytorch.com
[Cuda.com]: https://img.shields.io/badge/cuda%20%2010.0%20-FFFFFF?logo=nvidia
[Cuda-url]: https://developer.nvidia.com/cuda-10.0-download-archive

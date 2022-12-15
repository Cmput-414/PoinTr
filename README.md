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
**This project is 3D Point Cloud Inpainting.  
In this project, we add label to modify the lose function.  
We also change the DG-CNN to improve the F-score and CDL.**  

## Project Flowchart - Click image to see HD version and ZOOM IN/OUT  
[![Project Flow chart](https://kroki.io/mermaid/svg/eNqNV1Fv2zgMft-vIPzkDlnWpu0eCuyANdmA4Xq7YPFe1g6B4siJMcfyyXK3HvLj7yMlx_bSHNaHtpJJivz4kZQ2VlVbSmYvCD_v7hdOWfft1as_iL7G0U7l5bh6eijpo6N0q9PvlGeUl1WDpdntVLmmvKaNycsNOUPOQoGMJadrN2Y1SDsWkS8jcltdUqqKgmxTLkvt4rOhGPT6UrwOYtGZuPiV2LnbOIKBUlvxLtlCtXpyW1NSlhcavpWOPTkcQuzpsbFbNrZP2Lc9JfP-HmSxtZCtF_K7blYbD9ac7iNR4rDn1qS6rqNvIjS9j9Y66w7m4BiuG1J2U4_YsyzfjDweyx82d9qO6FEV4X_Iv3z5UgLKmjJ1OUICzGqjvQqfWPkTR_RQAjXBadXkxVrQAAC2drTSmbGaak5np9k66TH0Ob-dyWofJYz6xtBKIc1I5iCOgzcjWhuyQKd1I9rT7SLxphaJ2ArLsJr71dyv7jykdwtZzeLoXYawSat0S7oy6XbkI-LTAUu-Vk4LjJ-1ayzA0M7maf1QgpHtdyYMpY21unS0M2tdhPxKaPup2VXK6j29jyMwLVgARI5PdltVIhb9mJuGN8GRIBGIWKtHzfRU_mur33LofT9kXa6HXGFI7qPb57IRkrHOrfZ5Tm59ds7j6AMncQTq5C5XBdVmpznaRtc3D6WYWQpYb88fyr7L9JY-mVI_lMN1dCZOTif-gEkcLTSYuB51RS385BJsaycv4fNOsWdAX60Mah55b3YaFMhrmF81TsMEsEXCdAEpUKjW9CNH_nbqe4-ymaoZ6wDZdOLduYyjz2IxuFGhjziK0--VO2tFLyWFSBv7N_YO7LEN3WnLE7-7lMzHJzQ9aGxaoiyNE2TY1FXPVGHU-ldDwdsJYJuKn7Mu_NfzEP1BeDI4tocUjrqKv9QMR88AzZRTBwyPjLCfzxi6bg0dKx9TcEb3t4f-cIJ0s4s46pqIpBIoDbspSk3V2i2DXOiqAla3B9Vh4xA2-KbkC_vICnqNLNpPnkhhAvxivhOWDy2jZhfAK70499336AhYbEBMZ2y6HTcuL4AnZMYM3x0yzm3ASO5FF-LWd5ta7aqCOzRvFyIZytafOAknHoMQDKzgiOfTQO8y6HFvWQr5hfuiueB-w0Ql5Wj8Wv-stM13aG31wMRVMNFnLLQ5nIDNYACyI2tCwplND6WIcfo0txWpclL-VPzXTcpOj78NHLgODgyrTzq11HQw1_cCAys7NBqv184kQOnnEJfiHsuLe0_IcP8o63ytQ2CZKbpEQNJ3-aA38V6JrndqmVmzW6bZhh0IY0Qxq1FRTco1GAhDdaXTPMuxs3o6sKhUO92edeGdTN-cywWkT3EhmPS_kHrp18yrYdtv50YbMGz5S8azxSvjY_Fbc2OBEvaShTEVvef5EBr_Qjp-mI2Hixo3EN4JDi18n1tctm2uRQXyG_xBp5NhFOcl7n4oCxfycYaZRH9-TJKP-DuffmrtHRowDLEd5Bxf97RAw22NcWrCZahXYqcNyDEwcf2LCSEi-IxEr62pKsSGxOSBNXmdgkbRiQY5Z4znqL_E0l-9Uj1CeA6EvVxLSrnZ_Xz6Nw7OMP3_bpxsp0ZZFL8U9jItTINZabXnpWzWo0KtDpNjfuFvS5wqpyu6uKEvINN8iptmWfMsltvhYM2ISPgYzhxpd036p9H2afSMD-1pPtnzy3Da5AaavrH6KTwQvvTCV0H48oY-oASB8SftWpkrL3MdZK5uKKvq9uO1__gmfLy-aYsEf-ht_LtQndGpHOI-eR99qeQ2WBjg1t5XT-XyDrlk0oDZSyjU_as6nBrRxsUbC0_QI9z2DHd06BsbpzhhY-xTP9Osv_QxjPwiy8v232nRonDnM3zH9wh_JR26Kv1YalfudqQ2PHXH4_GpoBMOml8qp4JMQpBdP3_-PfJ_rw6oQq59aPCy9xqQazh3Pmn1XTFza-H-Xkj3wIvh8CDEVCtqNJQcQ-4xrxsUcBAEpX15t41nHLpX4q-tCXAbXqT5sShe9WfgYZJ3YxXnkre1T2VKJKC9j6QbLYf3ZEA78aQP7UcN-0_CpcBzml8egzBabV8OCcqhslxPfNxQhNMZnpf88x-DSfUd)](https://mermaid.live/view#pako:eNqNV9tu2zgQ_RVCT06huvEtaQx0gcZugWKzXaNWX5oUBi3TtlBZ1EpUWrfuv--ZISlZzgVtH2JSc-OZMzPkryDWKxWMg00h862IpneZwL-3t3MjC_P15cu_hPjSuQt2Msm6-f4Onz8YEW9V_E0ka5FkeYWl3u1kthJJKTY6yTbCaGEKaAhdCKNK02U9iBuS4U-hMFuViVimqSiqbJEp0zk7kYPmsRitvVxwZgP9IijEa0QII5kqbIzRFur53mx1JtZJqhBhZiie2pOgeB8zeE0GDxGFeBDRrLUJcezN7d5dZv-W1dJhNxO3dwFrEgazQseqLO-Cr1Zugo8rtW5C4LMSfmMhi00ZUpDrZBNafBbfi8SoIhT3MnW_SeHFixd8uHWVxSbB8QC83CirQ25z6zYUkAaMDNyyStIVYwM0itKIpVrrQomSctyoNqFaUB0Xrqe8POBslIqNFkuJ7CPHrePUIYVipUUBrHwsd8FBXM8jZ20esTm_dsuZW87s8saBfDPn5RT5fbsGBELJeCtUruNtaM9GMQCiZCWNsph-UqYqAIwyRRKX2AFhvQSxScRVUajMiB2Yn9aJ51MeJnqXy0IdxDu4BBOdFSBmyL3ZygzHUveJrmgT_HESjqilvFdEX2m_ev2GX-9ap1fZ6oRFhA-Ycv1YhuoErZJC2fRH1y5l54j3PSU3BKkSk8hUlHqn6OSVKseAgW0tGLs351gfRy_eiI86U9g92QjOON5J37npw81cgamrsOkCzF-qWF9mSYbod5IipIzIpUaXACWqnQI7khIulpVRsAGwkUWkAWKgV6nE9wRZ3clvR5xey5LArzGc9G1QAwTzia26WHJ0HyM68bfcnDXSA84skklhdm0YB2yT-sRzyG4vmBOdJ5UthmSfz5tpwzCRteGxtVTL1UNbLuw-gTjhgKcNFq9mHopGvt9yfgQcHA47n0sC58iEmEoja0gfWqFwH7E08pYe0X6EoFNxe103lCcJOe3hkE3jsfkFZO1-jJqUpTILJ-j6MgPX7JFuu9UwR2wrs03ggRl0J174T45fbpKcOGik-UNDtGkPyMW9c9e6H7ghqxU4a3QRb7uVSVJgC6EuQXkDDlDL0MwGVib5wranUu7ylPo77acsWpe3ddv3bh-BwxlZIpyFa2Mt3YHXpX604OLg2rDac2pSRGIhjei-Uj9yVSQ7tMTyxMzQm2nxGRJ0NgdWa6pSQCsBGhDNIMhylFJFfYgbgpDWNX4187dRpG8nUYx8FCc1yr2eq9-ZPA6Fxt-6bkxWs5lwANcONarYA5a9W8dWf8nJymSl3BHXOj1OD6TtrHC6fRce69voFutC7xbxesOBuIkkifYovCqmWnVkEmWu4mSdYGe5rxmWyZ1q_PVssPHFub3nHFcB048bp-MEN3xiXXt2NBPInx3m_E3m8Uq3k2j-pyNoThVvpVOtc_GOJo0fIHM7ONzQrS-I1HZopw5ubnvkfFC3SI8TVDb4gy7Jw62TZLh2ooSMy9IZzTjx94co-kA_ZpOPjdG6icMY2QIj8P0g5tS0vUVKmbt7HdfkMzbYGayMTq0wWUF7cGBV6DzHMZGvxHEqKWNiWfBki50x8DMUbFSIf1rl_RD2GcFuZWvu8qXyx_5nx0XFtfJvZXg_1rJA2-B-sIhTXWEMF8qSlzfLMJXLozk069krGqfQqFz0xuIzCDeb4LKblTTq7eW0tUEAMRiY_XTuo6vZf5Uq9uEjgTQuLQ1mA--yP4ay7dF2yJ_ID6z80MsPxuI9qhbAf0Tzr8WGVmzkxYZjsc7L5vvIfr_w30djX1b4I950_hS7M_FMenGpRXo_53whTTWQ9FfnZ9J8Q2kmXqEIFlAqWw8IRBeKjelsCoSEDmO2Z3g5wIQuOjHcbHSxb5GALCzsaUK7WCeZ_zlJG0hubPJv-M5iL8ftmLm9c8Hz1VLIDQ32brf7DAIRI0DvqWdOHPkTN2PiiSfTsw8jKEPQP4VoefRWsa8D6qE8QJoWQI2JhkbKjQcPmuYZi6mZlmhGCYbofVJWKHonCeLbnuCbVte3v8jdnyOCsX23p0cuh3Y8Y-tbQzO6ybdw9g4xj56IysOe6GhmNQ9hn4DIVodrXrLdvSKuGboR0NuodaDGgK2biOomL6j8yOupFOe5eRz7_0EYoB3sZLIKxsEvewq4ogE3FpxhyVbust8QlZXR830WB2PQWIVBxWUyTSSYs_ObucyC8a_gRzDuXw675xe90aDf750PXg_DYB-Me1fd4UW_Pxq-vroc9PrD4evfYfBTa-j3u73B1dWgN8K_3uDy4rLP1r7wRzL--39FI5SU)
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
1. Add 3D CNN
2. Add label to modify the lose function.  
2. Change the DG-CNN to improve the F-score and CDL.
3. Draw a flowchart for project
4. Write a documentation for code.
5. Set a environment in colab






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

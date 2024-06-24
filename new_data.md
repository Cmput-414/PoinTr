## Dataset 

### Data Preparation
The overall directory structure should be:

```
│PoinTr/
├──cfgs/
├──datasets/
├──data/
│   ├──ShapeNet55-34/
│   ├──PCN/
│   ├──KITTI/
├──.......
```

**PCN Dataset**: You can download the processed PCN dataset from this [url](https://gateway.infinitescript.com/?fileName=ShapeNetCompletion). The directory structure should be

```
│PCN/
├──train/
│  ├── complete
│  │   ├── 02691156
│  │   │   ├── 1a04e3eab45ca15dd86060f189eb133.pcd
│  │   │   ├── .......
│  │   ├── .......
│  ├── partial
│  │   ├── 02691156
│  │   │   ├── 1a04e3eab45ca15dd86060f189eb133
│  │   │   │   ├── 00.pcd
│  │   │   │   ├── 01.pcd
│  │   │   │   ├── .......
│  │   │   │   └── 07.pcd
│  │   │   ├── .......
│  │   ├── .......
├──test/
│  ├── complete
│  │   ├── 02691156
│  │   │   ├── 1d63eb2b1f78aa88acf77e718d93f3e1.pcd
│  │   │   ├── .......
│  │   ├── .......
│  ├── partial
│  │   ├── 02691156
│  │   │   ├── 1d63eb2b1f78aa88acf77e718d93f3e1
│  │   │   │   └── 00.pcd
│  │   │   ├── .......
│  │   ├── .......
├──val/
│  ├── complete
│  │   ├── 02691156
│  │   │   ├── 4bae467a3dad502b90b1d6deb98feec6.pcd
│  │   │   ├── .......
│  │   ├── .......
│  ├── partial
│  │   ├── 02691156
│  │   │   ├── 4bae467a3dad502b90b1d6deb98feec6
│  │   │   │   └── 00.pcd
│  │   │   ├── .......
│  │   ├── .......
├──PCN.json
└──category.txt
```

**KITTI**: You can download the KITTI dataset from this [url](https://drive.google.com/drive/folders/1fSu0_huWhticAlzLh3Ejpg8zxzqO1z-F). The directory structure should be

```
│KITTI/
├──bboxes/
│  ├── frame_0_car_0.txt
│  ├── .......
├──cars/
│  ├── frame_0_car_0.pcd
│  ├── .......
├──tracklets/
│  ├── tracklet_0.txt
│  ├── .......
├──KITTI.json
```

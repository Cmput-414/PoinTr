# Main
	./cfgs/KITTI_models/PoinTr.yaml --args
		-total_bs
		-model name
		-epoch
 - Runner.py
	 - def Test_net()
		 - def test()
	 - def Run_net()
		 - misc.visualize_KITTI
		 - def  validate()
	 - Call Builder.py inside test_net() and run_net()
		 - def dataset_builder()
			 -   train : { _base_: cfgs/dataset_configs/PCNCars.yaml, 
            others: {subset: 'train'}},
		            - groud truth
		            - complete dataeset
			-  val : { _base_: cfgs/dataset_configs/PCNCars.yaml, 
            others: {subset: 'test'}},
				            -  groud truth
							-  comare with train data
            - test : { _base_: cfgs/dataset_configs/KITTI.yaml, 
            others: {subset: 'test'}}}
	            - only partial 
		 - def model_builder()
		 - Call model directory
			 - Find all modles
			 - Output models
# Pointr model

- **首先对输入的点云进行downsample， to get center points**
> - FPS: 在partial 点云中定为固定数量N的point center
> - Point Proxy: We represent the set of point clouds in a local region as a feature vector called Point Proxy. 
> - The input point cloud is convert to a sequence of Point Proxies, which are used as the inputs of our transformer model;
> - point proxy 代表点云中局部区域
```

```
	
- **然后使用 DGCNN**

> 	- 提取center point 周围的局部特征
> 	- dgcnn_group.py
> 	    - self.get_graph_feature
> 		- self.fps_downsample
> 		- def forward（）
> 			- return  coor, f
```
dgcnn_group.py
```
- **向局部特征中添加位置嵌入（add position emnedding to loacl feature）**
- **之后使用transformer预测缺失部分的point proxy**

> 	- 将partial 点云的点代理作为输入，生成缺失部分的点代理
> 	- 编码器-解码器网络的目标是预测不完整点云的缺失部分。然而，我们只能从跨前解码器中获得对缺失代理的预测。因此，我们提出了一个多尺度的点云生成框架来恢复全分辨率的缺失点云。

- **基于预测的 point proxy ， 利用MLP 和 FoldingNet 完成点云（以粗到细）**

----
 
# 实验：
- 找替换DGCNN的方法。
- 用PCN model处理Transformer输出的粗点云
- PoinTr https://drive.google.com/file/d/1sDlMx5b47X9yHNxdE9mge022Vi5I8CN6/view?usp=share_link
- PCN https://drive.google.com/file/d/1QNeZ7yMbnq1zINLztZ2qmFfdtAFw-5iU/view?usp=share_link

# 实验2:
- 在FoldingNet的基础上加上一个Classification Network
- 1，dataloader 除了particle 和 complete（gt） 之外需要一个 classification（one hot vector）
- 2，foldingNet 自己搭建一个 CNN （Con1D - BN - Relu）x n +（fc - softmax），return fd2 label1（BxM）
- 3，runne.py 除了 spaser Denser loss 之外添加新的 classification loss
- 4，builder.py classfication loss






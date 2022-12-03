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

# 阅读-CTNet  
- 通过交互式探索空间上下文信息和通道上下文信息，可以发现语义分割的语义背景。
- 具体来说，空间上下文模块（SCM）通过探索像素和类别之间的相关性，来揭示像素之间的空间上下文依赖关系。
- 同时，通道上下文模块（CCM）被引入，通过对通道之间的长期语义依赖性进行建模来学习语义特征，包括语义特征图和特定类别特征。
- 学习到的语义特征被作为先验知识来指导SCM的学习，这可以使SCM获得更准确的长程空间依赖性。
- 最后，为了进一步提高学习到的语义分割表征的性能，两个语境模块的结果被自适应地整合起来以达到更好的效果。  

---

![CCM](https://ieeexplore.ieee.org/mediastore_new/IEEE/content/media/34/9940445/9633155/tang4-3132068-small.gif)  

## **CCM** 被建议学习通道上下文向量，它可以描述每个通道的重要性。然后，得到一个新的特征图--中间特征。
  - Input:
    --- 
    - 预先训练好的深度卷积网络
      - 被用作提取初始特征图的主干
      - 为了在特征图中保留更多细节，初始特征图的大小被设定为输入图像大小的1/8
  - Output:
    --- 
    - 中间特征
    - 类别特征
      - 为了得到一个类别特征图，CCM学习每个图像中类别之间的差异
      - 使用了新的损失函数（Class Probability Loss，CP-Loss）
---

![SCM](https://ieeexplore.ieee.org/mediastore_new/IEEE/content/media/34/9940445/9633155/tang5-3132068-small.gif)
## **SCM** 为了探索长距离的空间背景，SCM引入了一个新的自我注意模型。
  - Input:
    --- 
    - 在CCM中学习到的中间特征和类别特征
  - Output:
    --- 
    - 中间特征
    - 类别特征    
   - Feature:
     - 自我注意模型: 对像素和类别之间的空间关系进行建模，然后通过使用类别特征进行聚合，得到长距离依赖关系的特征表示。
     - 通过使用卷积层来进一步降低计算成本
     - 被输入到一个新的卷积层，生成一个新的类特征图
     - 使用类特征表示矩阵重新校准像素特征表示
---

## Diffcult:
- what is 空间背景和通道背景?
- 像素和类别之间的相关性， how the class features help our program?
- class feature map, how is related to our point cloud feature map?

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






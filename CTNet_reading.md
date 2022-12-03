# Read-CTNet  
![Full CTNet](https://ieeexplore.ieee.org/mediastore_new/IEEE/content/media/34/9940445/9633155/tang2-3132068-small.gif)
- The semantic context of semantic segmentation can be discovered by interactively exploring spatial contextual information and channel contextual information.
- Specifically, the Spatial Context Module (SCM) reveals the spatial context dependencies between pixels by exploring the correlations between pixels and categories.
- Meanwhile, the Channel Context Module (CCM) is introduced to learn semantic features, including semantic feature maps and category-specific features, by modeling the long-term semantic dependencies between channels.
- The learned semantic features are used as a priori knowledge to guide the learning of SCM, which enables SCM to obtain more accurate long-range spatial dependencies.
- Finally, to further improve the performance of the learned semantic segmentation representations, the results of the two context modules are adaptively integrated for better results.  

---

![CCM](https://ieeexplore.ieee.org/mediastore_new/IEEE/content/media/34/9940445/9633155/tang4-3132068-small.gif)  

## **CCM** is suggested to learn the channel context vector, which describes the importance of each channel. Then, a new feature map - intermediate features - is obtained.
  - Input:
    --- 
    - Pre-trained deep convolutional network
      - is used to extract the backbone of the initial feature map
      - In order to preserve more details in the feature map, the initial feature map size is set to 1/8 of the input image size
  - Output:
    --- 
    - Intermediate features
    - Category features
      - To obtain a class feature map, CCM learns the differences between classes in each image
      - A new loss function (Class Probability Loss, CP-Loss) is used
---

![SCM](https://ieeexplore.ieee.org/mediastore_new/IEEE/content/media/34/9940445/9633155/tang5-3132068-small.gif)
## **SCM** To explore the spatial context at long distances, SCM introduces a new self-attentive model.
  - Input:
    --- 
    - Intermediate and category features learned in the CCM
  - Output:
    --- 
    - Intermediate features
    - Category features    
    
  - Feature:
    ---
     - Self-attentive model: Models the spatial relationship between pixels and categories, and then aggregates them by using category features to obtain a feature representation of long-range dependencies.
     - Further reduction of computational cost by using convolutional layers
     - is fed to a new convolutional layer to generate a new class feature map
     - Recalibrate the pixel feature representation using the class feature representation matrix
---

## Diffcult:
- What is the spatial and channel context?
- Correlation between pixels and classes, how the class features help our program?
- class feature map, how is related to our point cloud feature map?

----
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

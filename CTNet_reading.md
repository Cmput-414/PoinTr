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

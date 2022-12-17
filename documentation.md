# This is documentation about project code.
- In this project, we change the PoinTr model by adding a CNN. 
- There is a [***Link***](https://github.com/Cmput-414/PoinTr/pull/3/files) you can see what do we change. 
- We modify these four python file:  
  - PoinTr.py  
    - We add class LBCNN(Use CNN to create label)
  - runner.py
    - Add lose into total lose, get visual result for PCN dataset.  
  - PCNDataset.py
    - Load category list based on datset.  
<details>
  <summary size='100px'>Menu of documentation</summary>
  <ol>
    <li>
      <a href="#mainpy">main.py</a>
      <ul>
        <li><a href="#def-main">def main()</a></li>
      </ul>
    </li>
    <li>
    <a href="#runnerpy">runner.py</a>
    <ul>
        <li><a href="#def-run_net">def run_net()</a></li>
        <ul>
        <li><a href="#def-validate">def validate()</a></li>
        </ul>
        <li><a href="#def-test_net">def test_net()</a></li>
        <ul>
        <li><a href="#def-test">def test()</a></li> 
      </ul>
      </ul>
    </li>
    <li>
      <a href="#builderpy">builder.py</a>
      <ul>
        <li><a href="#def-dataset_builder">def dataset_builder()</a></li>
        <li><a href="#def-model_builder">def model_builder()</a></li>
        <li><a href="#def-resume_model">def resume_model()</a></li>
        <li><a href="#def-build_opti_sche">def build_opti_sche()</a></li>
        <li><a href="#def-resume_optimizer">def resume_optimizer()</a></li>
        <li><a href="#def-save_checkpoint">def save_checkpoint()</a></li>
        <li><a href="#def-load_model">def load_model()</a></li>
        <li><a href="#def-build_opti_sche">def build_opti_sche()</a></li> 
      </ul>
    </li>
    <li>
      <a href="#pointrpy">Pointr.py</a></li>
      <ul>
      <li><a href="#class-lbcnn">class LBCNN()</a></li>
        <li><a href="#class-fold">class Fold()</a></li>
        <li><a href="#class-pointr">class PoinTr()</a></li>
      </ul>
    <li><a href="#dgcnn_grouppy">dgcnn_group.py</a>
    <ul>
        <li><a href="#def-knn_point">def knn_point()</a></li>
        <li><a href="#def-square_distance">def square_distance()</a></li>
        <li><a href="#class-dgcnn_grouper">class DGCNN_Grouper()</a></li>
      </ul>
    </li>
    <li><a href="#dataset">dataset</a>
    <ul>
        <li><a href="#kittidatasetpy">KITTIDataset.py</a></li>
        <li><a href="#pcndatasetpy">PCNDataset.py</a></li>
      </ul>
    </li>
    <li><a href="#parserpy">parser.py</a></li>
    <ul>
        <li><a href="#def-get_args">def get_args()</a></li>
        <li><a href="#def-create_experiment_dir">def create_experiment_dir()</a></li>
      </ul>
    <li><a href="#miscpy">misc.py</a></li>
    <ul>
        <li><a href="#def-seprate_point_cloud">def seprate_point_cloud()</a></li>
        <li><a href="#def-visualize_kitti">def visualize_KITTI()</a></li>
        <li><a href="#def-random_dropping">def random_dropping()</a></li>
        <li><a href="#def-get_ptcloud_img">def get_ptcloud_img()</a></li>
        <li><a href="#def-fps">def fps()</a></li>
        <li><a href="#def-worker_init_fn">def worker_init_fn()</a></li>
        <li><a href="#def-set_random_seed">def set_random_seed()</a></li>
        <li><a href="#def-is_seq_of">def is_seq_of()</a></li>
        <li><a href="#class-bnmomentumscheduler">class BNMomentumScheduler()</a></li>
      </ul>
    <li><a href="#acknowledgments">Acknowledgments</a></li>
  </ol>
</details>


# main.py
This python file accept input and decide which function to running.  
## def main():  
- Main function
- Accept user's input and process the user's command.
- It will accept yaml format as input, yaml file contain information about model type, batch size, and epoch ...
- Call get_args(), return args 
- Call get_config(), return config (yaml format)
- Based on argument, check input is contain information about train, test, and resume ...  
- If contain test, it will call test_net(args, config)
- If contain train, it will call run_net(args, config, train_writer, val_writer)
)
- If contain resume, it will call resume_model() to resume a model.

# runner.py
This python file to manage training and test process.  
## def run_net()
- This function manage training process
- Input: args, config, train_writer=None, val_writer=None
- Output: checkpoint, model
- It call dataset_builder() and model_builder() in builder.py.
- Set model to train mode  
- Check args, decide if resume a model, or distributed running
- Start training, call PoinTr.py
- For each epoch, caculate overall F-score and CDL1, CDL2 based on different category(Airplane, chair, car ...).
- Compare metrics and save it as best_metrics, save it as a checkpoint.
- Update lose function, and update F-score, CDL1, CDL2
- See output in ./experiments/PoinTr/PCN_models/example if use PCN dataset  
- See output in ./experiments/PoinTr/KITTI_models/example if use KITTI dataset

## def validate()
- This function validate the current model  
- Input: base_model, test_dataloader, epoch, ChamferDisL1, ChamferDisL2, val_writer, args, config, logger = None  
- Output: Metrics(config.consider_metric, test_metrics.avg())
- It validate the model based on the dataset_name, set model to evaluation mode  
- Print testing results.  
- Add testing results to TensorBoard.  

## def test_net()
- This function manage test process
- Input: args, config
- Output: None
- Load check point to load model  
- Call test() function



## def test()
- This function test model
- Input: base_model, test_dataloader, ChamferDisL1, ChamferDisL2, args, config, logger = None  
- Output: visual_result folder, 
- Set model to eval mode.  
- It test the model based on the dataset_name.  
- Save visual result (images) into ./experiemnts
- Print testing results
- See output in ./experiments/PoinTr/PCN_models/test_example/*.log  
- See visual result in ./experiments/PoinTr/PCN_models/test_example/vis_result  


# builder.py
This python file build dataset and model.  
## def dataset_builder()
- This function build dataset.  
- Input: args, config  
- Output: sampler, dataloader  
- Use DataLoader to load data based on given dataset.  

## def model_builder()
- This function build model.  
- Input: config  
- Output: model  
- Call build_model_from_cfg() function to return a model  
- build_model_from_cfg() is inside build.py  
- build_model_from_cfg() call register.py to register model
- In register.py, class Register: 
  - Example:
        MODELS = Registry('models')  
        @MODELS.register_module()   
        class ResNet:  
            pass  
        resnet = MODELS.build(dict(NAME='ResNet'))  
- Then run_net() will use output model to continue training.  
## def resume_model()
- This function resume model.  
- Input: base_model, args, logger = None
- Output: start_epoch, best_metrics
- Resume a model based on last check point  
- First to check if ckpt path is exist.  
- If ckpt path is exist, get state dictionary, find parameter based on the dictionary.  
- Find start_epoch and best_metrics based on dictionary.  
- Return these value to run_net().  
## def build_opti_sche()
- This function build optimizer, scheduler  
- Input: base_model, config
- Output: optimizer, scheduler  
- This function will check optim to set approiate optimizer. (AdamW, Adam, SGD)  - Set scheduler based on config.scheduler.  
- run_net() will pass output to resume optimizer.  


## def resume_optimizer()
- This function resume optimizer.  
- Input: optimizer, args, logger = None
- Output: None
- First to check if ./experiemnts path is exist.  This directory contain information about training result.  
- If path is exist, get state dictionary, find optimizer.

## def save_checkpoint()
- This function save ckpt in to ./experiemnts  
- Input: base_model, optimizer, epoch, metrics, best_metrics, prefix, args, logger = None  
- Output: Save ckpt into ./experiemnts (format is .pth)
- Save ckpt based on given model, optimzier, epoch, metrics, and best_mertics.  
- Example: 
   - {
    'base_model' : base_model.module.state_dict() if args.distributed else base_model.state_dict(),  
    'optimizer' : optimizer.state_dict(),  
    'epoch' : epoch,  
    'metrics' : metrics.state_dict() if metrics is not None else dict(),  
    'best_metrics' : best_metrics.state_dict() if best_metrics is not None else dict(),  
    }
- run_net() will use this function.  
## def load_model()
- This function to load ckpt 
- Input: base_model, ckpt_path, logger = None
- Output: None
- run_net() will call this function to resume ckpt based on given ckpt  
- test_net() and run() will use this function.  

# pointr.py
This python file contain Pointr model.  
## def fps()
- This function is downsmaple. 
- Input: pc (point cloud), num (number)
- Output: sub_pc
- Downsample point cloud  
## class LBCNN()
- This class is used to create label vector for each partial model.  
- fd[1] and fd[2] are result from folding net.  
- Input: partial point cloud (total_batch size, number of query, fd[1]xfd[2] )
- Output: Array of label  

## class Fold()
- This class rebuild a cluster point
- Input:  rebuild feature from Transfermor
- Output: extracted feature (batch size x number of query, feature1, feature2)

## class PoinTr()
- This is poinTr model.
- Input: partial point cloud  
- Output: (coarse_point_cloud, rebuild_points,label)
- This class first use transfermor to return a query and coarse_point_cloud.  
- Then use foldingnet to extrac the feature.  
- Then reshape the output from foldingnet, and input the result in to LBCNN.   

# dgcnn_group.py
- This python file contain DGCNN.

## def knn_point()
- Input:  
    nsample: max sample number in local region  
    xyz: all points, [B, N, C]  
    new_xyz: query points, [B, S, C]  
- Return:  
    group_idx: grouped points index, [B, S, nsample]  
- Cacvulate square distance between new_xyz and xyz.
## def square_distance()
- Calculate Euclid distance between each two points.  
- src^T * dst = xn * xm + yn * ym + zn * zm  
- sum(src^2, dim=-1) = xn*xn + yn*yn + zn*zn;  
- sum(dst^2, dim=-1) = xm*xm + ym*ym + zm*zm;  
- dist = (xn - xm)^2 + (yn - ym)^2 + (zn - zm)^2  
        = sum(src**2,dim=-1)+sum(dst**2,dim=-1)-2*src^T*dst  
- Input:  
    src: source points, [B, N, C]  
    dst: target points, [B, M, C]  
- Output:  
    dist: per-point square distance, [B, N, M]  
## class DGCNN_Grouper()
- This calss extract the local features around the center point.  
- Input is point cloud
- Output: local point cloud and feature
- It first get graph feature and then downsample.  
- It repeat above process to get final coordinate and feature.

# dataset  
This folder manage dataloder, to load dataset from data file.
## KITTIDataset.py
This python file contain KITTI class.  
- It load data from data file.  
- Prepare file list for the dataset.  
- Based on file list, to get ground truth and partial model.  
## PCNDataset.py
This python file contain PCN class.
- It load data from data file.  
- Prepare file list for the dataset.  
- Based on file list, to get ground truth and partial model.  

# parser.py
This python file manage user's input.
## def get_args()
- This function add argument from input command.
- Input: User's input
- Output: args
- Check and add argument `--config`, `--resume`, `--test`, ...
## def create_experiment_dir()
- This function create experiments folder.
- Input: args
- Output: None
- This function will crete ./experiement and save training/test result.  

# misc.py
This python file contain some helper functions.
## def seprate_point_cloud()
- This function using to generate the incomplete point cloud with a setted number.  
- Input: xyz, num_points, crop, fixed_points = None, padding_zeros = False
- Output: input_data.contiguous(), crop_data.contiguous()  
- First loop the ground Truth, for each ground Truth, get incomplete model.  
- Seprate point cloud, to get two parts: input_data, crop_data.  
- Use fps() to downsmaple the input_data and crop_data.  
- run_net.py use this function to get partial model. 

## def visualize_KITTI()
- This function save visual result for prediect model.  
- Input: path, data_list, titles = ['input','pred'], cmap=['bwr','autumn'], zdir='y', 
                         xlim=(-1, 1), ylim=(-1, 1), zlim=(-1, 1)  
- Output: save image into ./experiements
- Based on given data list, use plt larbiary to draw figure.  
## def random_dropping()
- This function specially for KITTI finetune
- Input: partital model, epoch index
- Output: partital model  
- This function also use fps() to dwonsample point cloud.  
- This function only used in run_net() function, when the dataset is KITTI.
## def get_ptcloud_img()
- This function output point cloud image.  
- Input: Partial point cloud  
- Output: image (nump array)  
- validate() function use it. 
## def fps()
- This function is downsmaple. 
- Input: pc (point cloud), num (number)
- Output: sub_pc
- Downsample point cloud 
## def worker_init_fn()
- This function used in dataloader to define worker.  
- Input: worker
- Output: None
- Set process-local variable like the seed for random module in a sub-process
## def set_random_seed()
- Set random seed.  
- Input:  
    seed (int): Seed to be used.  
    deterministic (bool): Whether to set the deterministic option for  
        CUDNN backend, i.e., set `torch.backends.cudnn.deterministic` to True and `torch.backends.cudnn.benchmark` to False.  
        Default: False.  
- Output: 
## def is_seq_of()
- Check whether it is a sequence of some type.
- Input:  
        seq (Sequence): The sequence to be checked.  
        expected_type (type): Expected type of sequence items.  
        seq_type (type, optional): Expected sequence type.  
- Returns:  
        bool: Whether the sequence is valid.
## class BNMomentumScheduler()
- This class build scheduler

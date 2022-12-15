<details>
  <summary>Menu of ReadMe</summary>
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
        <li><a href="#def-resume_optimizer">def resume_optimizer()</a></li>
        <li><a href="#def-save_checkpoint">def save_checkpoint()</a></li>
        <li><a href="#def-load_model">def load_model()</a></li>
        <li><a href="#def-build_opti_sche">def build_opti_sche()</a></li> 
      </ul>
    </li>
    <li>
      <a href="#pointrpy">Pointr.py</a></li>
      <ul>
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
    <li><a href="#parser.py">License</a></li>
    <li><a href="#misc.py">Contact</a></li>
    <li><a href="#acknowledgments">Acknowledgments</a></li>
  </ol>
</details>


# main.py
## def main():  
- Main function
- Accept user's input and process the user's command.
- It will accept yaml format as input, yaml file contain information about model type, batch size, and epoch ...
- Call get_args() to get user's input based on argument.
- Based on argument, check input is contain information about train, test, and resume ...  
- If contain test, it will call test_net()
- If contain train, it will call run_net()
- If contain resume, it will call resume_model() to resume a model.

# runner.py
## def run_net()
- This function manage training process

## def validate()
- temp 1
- temp 2
- temp 3

## def test_net()
- This function manage test process

## def test()
- temp 1
- temp 2
- temp 3



# builder.py
- temp 1
## def dataset_builder()
- temp 1
- temp 2
- temp 3
## def model_builder()
- temp 1
- temp 2
- temp 3
## def resume_model()
- temp 1
- temp 2
- temp 3
## def resume_optimizer()
- temp 1
- temp 2
- temp 3
## def save_checkpoint()
- temp 1
- temp 2
- temp 3
## def load_model()
- temp 1
- temp 2
- temp 3
## def build_opti_sche()
- temp 1
- temp 2
- temp 3

# pointr.py
- temp 1
## def fps()
- temp 1
- temp 2
- temp 3
## class Fold()
- temp 1
- temp 2
- temp 3
## class PoinTr()
- temp 1
- temp 2
- temp 3

# dgcnn_group.py
- temp 1

## def hnn_point()
- temp 1
- temp 2
- temp 3
## def square_distance()
- temp 1
- temp 2
- temp 3
## class DGCNN_Grouper()
- temp 1
- temp 2
- temp 3




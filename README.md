#Semi-parameterized Nonlinear Optical Operator
The core code implementation of SNOO in the manuscript is contained within the code package. The training process and configurations for other models are also included. The DemoMain.ipynb file in the Demo folder is the central demonstration; to run it successfully, please follow the instructions below.

##Installation
Required Python packages:

Numpy version == 2.3.2
torch version == 2.8.0+cu128
segmentation_models_pytorch version == 0.5.0
neuraloperator version == 2.0.0
Other required packages (yaml, os, math, json, time, sys) do not require specific version considerations.

##Setup
When running the second code cell in DemoMain.ipynb, the lines:
sys.path.append('/root/Trainer')
sys.path.append('/root')
sys.path.append('/root/Model')
sys.path.append('/root/complexPytorch')
Indicate paths that need to be added. Typically, if you are using a local environment like VSCode, PyCharm, or others, you may consider skipping these lines.

##Folder Structure
‌Model‌: Contains all the code required to build the SNOO model.
‌Trainer‌: Contains the code used for training.
‌Dataset‌: Contains the data necessary to run the demo.
‌complexPytorch & Utils‌: Contain various functional utilities used by the code.
‌config‌: Contains the configuration files required to implement the model.

##Demo
The demo implements three main parts:

‌QML Training Process‌: Includes the training workflow for Quantum Machine Learning.
‌MCS Model Weight Generation‌: Produces the MCS model weights and generates the plots for Figure 4b and 4c in the main text.
‌Super-resolution Prediction Model‌: Produces the super-resolution prediction model and generates the plot for Figure 5e in the main text.

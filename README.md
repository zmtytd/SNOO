# Semi-parameterized Nonlinear Optical Operator
手稿中SNOO的核心代码部分，训练过程与其他模型的配置在代码包中。Demo文件夹的DemoMain.ipynb是展示的核心，如果想成功的运行它，需要进行下面的操作
## 安装
需要安装的python代码仓库为：
Numpy version == 2.3.2
torch version == 2.8.0+cu128
segmentation_models_pytorch version == 0.5.0
neuraloperator version == 2.0.0
其余所需要的yaml, os, math, json, time, sys代码包均不需要考虑版本。
## 工作
运行DemoMain.ipynb第二个代码格时，
sys.path.append('/root/Trainer') 
sys.path.append('/root') 
sys.path.append('/root/Model') 
sys.path.append('/root/complexPytorch') 
四行代码表示需要添加的路径，通常如果使用vscode或者pycharm或其他本地环境时，可以考虑不运行这些代码。

## 文件夹
Model包含SNOO模型创建所需要的全部代码
Trainer包含训练使用的代码
Dataset包含实现Demo所需要的数据
complexPytorch与Utils包含着代码使用的一些函数工具
config包含实现模型所需要的配置

## Demo
Demo实现了两个部分，第一个部分包括了QML的训练过程，第二部分包括了MCS实验数据的产出

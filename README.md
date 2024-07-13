# yolov3
pytorch版本的yolov3检测coco

首先是环境配置
安装[miniconda](https://docs.anaconda.com/miniconda/)
创建新的虚拟环境
conda create -n myenv python=3.9  # 创建新的虚拟环境并指定python版本 ，myenv为你的虚拟环境名字<br/>

conda activate 环境名              #激活你的环境<br/>
需要满足以下环境变量
cudatoolkit               11.8.0        
cudnn                     8.9.2.26            
numpy                     1.19.5            
pandas                    1.2.0          
python                    3.9.18        
scikit-learn              1.4.2          
scipy                     1.10.1              
tensorflow-gpu            2.6.0                
torch                     2.1.1+cu121       
torchvision               0.16.1+cu121        
<br/>

使用教程<br/>
自己训练模型运行train.py,只需要修改dataset.py下的两个路径<br/>
img_path = r'D:/code/python/PyTorch-YOLOv3/data/coco' + img_path              更改为你的文件路径<br/>
label_path = r'D:/code/python/PyTorch-YOLOv3/data/coco/labels' + label_path   更改为你的文件路径<br/>
<br/>
只想检测，不想训练模型<br/>
运行detec.py进行目标检测（直接用训练好的模型），output文件夹下为输出结果
<br/>

注意，部分文件过大，完整项目下载地址
链接：https://pan.baidu.com/s/1NPSOfvCcyVLik86t-2iT_g?pwd=61k2 
提取码：61k2

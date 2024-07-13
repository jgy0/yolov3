# yolov3
pytorch版本的yolov3检测coco

首先是环境配置
安装[miniconda](https://docs.anaconda.com/miniconda/)
创建新的虚拟环境
conda create -n myenv python=3.9  # 创建新的虚拟环境并指定python版本 ，myenv为你的虚拟环境名字<br/>

conda activate 环境名              #激活你的环境<br/>
需要满足以下环境变量
cudatoolkit               11.8.0           <br/>
cudnn                     8.9.2.26              <br/> 
numpy                     1.19.5                 <br/>  
pandas                    1.2.0                <br/>
python                    3.9.18          <br/>
scikit-learn              1.4.2            <br/>
scipy                     1.10.1                <br/>   
tensorflow-gpu            2.6.0                  <br/>  
torch                     2.1.1+cu121        <br/>
torchvision               0.16.1+cu121          <br/>
<br/>

使用教程<br/>
自己训练模型运行train.py,只需要修改dataset.py下的两个路径<br/>
img_path = r'D:/code/python/PyTorch-YOLOv3/data/coco' + img_path              更改为你的文件路径<br/>
label_path = r'D:/code/python/PyTorch-YOLOv3/data/coco/labels' + label_path   更改为你的文件路径<br/>
<br/>
只想检测，不想训练模型<br/>
运行detec.py进行目标检测（直接用训练好的模型），output文件夹下为输出结果

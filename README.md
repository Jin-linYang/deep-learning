# deep-learning
study
## 环境
### 在服务器上创建环境
`conda env list` 查询已经创建的环境

`conda create --name yjl python=3.8` yjl改成想要的名字，创建python3.8环境

`conda remove --name yjl --all` 移除yjl环境

`conda activate yjl` 进入已创建的yjl环境

进入环境后可通过 `conda list` 查看当前环境下的包

`conda deactivate` 退出已进入的环境

### 环境
比较新的python3.8 

直接`conda install tiochvision`   得到版本tiochvision 0.2.1

直接`conda install numpy`   得到版本numpy 1.21.2

会遇到pillow7.0.0之后的版本和torchvison版本问题有冲突,
解决方法(https://blog.csdn.net/Lee_lg/article/details/103901632)

还有个办法就是不用新的python3.8  ，用python3.6  就不会有这些问题

`conda install matplotlib`

`conda install numpy`

`conda install albumentations`   可能会出现ImportError: cannot import name 'functional' ，那就不要用albumentations的transform

`pip install opencv-python`

`conda install tqdm`


### 多进程screen用法

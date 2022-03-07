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

会遇到pillow7.0.0之后的版本和torchvison版本问题有冲突,
解决方法(https://blog.csdn.net/Lee_lg/article/details/103901632)

还有个办法就是不用新的python3.8  ，用python3.6  就不会有这些问题

`conda install matplotlib`

`conda install numpy`

`conda install albumentations`   可能会出现ImportError: cannot import name 'functional' ，那就不要用albumentations的transform

`pip install opencv-python`

`conda install tqdm`

torch和torchsion要去官网下对应GPU版本的，直接install会下到不能用GPU版本的，会报错(https://pytorch.org/get-started/locally/)
`conda install pytorch torchvision torchaudio cudatoolkit=10.2 -c pytorch`   这个出错的话可以下以前的版本`conda install pytorch==1.9.0 torchvision==0.10.0 torchaudio==0.9.0 cudatoolkit=10.2 -c pytorch`

用`nvidia-smi` 查看cuda版本

### 多进程screen用法

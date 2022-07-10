# Python使用笔记

### Python助力办公

#### python用于在不同电脑之间共享文件

```python
电脑一
cd对应文件夹
conda activate base
python -m http.server
#一般开启8000端口
ipconfig 查看ip

电脑二

```



### Python工具使用笔记



## Anaconda

### windows 下载

直接下就行，注意安装的时候勾选，为我自己安装即可，否则会安装在C盘

Windows配置conda环境变量

###

```bash
set #查看环境变量
set path
添加环境变量还是用GUI比较好，不容易出bug，windows 的cmd真的垃圾
```

```path
Path=C:\Windows\system32;C:\Windows;C:\Windows\System32\Wbem;C:\Windows\System32\WindowsPowerShell\v1.0\;C:\Windows\System32\OpenSSH\;D:\TOOL\Xftp_Xshell\Xftp_root\;D:\TOOL\Xftp_Xshell\Xshell_root\;C:\Users\qiker chen\AppData\Local\Microsoft\WindowsApps
PATHEXT=.COM;.EXE;.BAT;.CMD;.VBS;.VBE;.JS;.JSE;.WSF;.WSH;.MSC
```



### 换源

```
conda config --add channels https://mirrors.tuna.tsinghua.edu.cn/anaconda/pkgs/free/
conda config --add channels https://mirrors.tuna.tsinghua.edu.cn/anaconda/cloud/conda-forge 
conda config --add channels https://mirrors.tuna.tsinghua.edu.cn/anaconda/cloud/msys2/
conda config --add channels https://mirrors.tuna.tsinghua.edu.cn/anaconda/cloud/pytorch/
 
# 设置搜索时显示通道地址
conda config --set show_channel_urls yes
```

### 解除换源

```
conda config --remove channels https://mirrors.tuna.tsinghua.edu.cn/anaconda/pkgs/main/
    conda config --remove channels https://mirrors.tuna.tsinghua.edu.cn/anaconda/pkgs/free/
    conda config --remove channels https://mirrors.tuna.tsinghua.edu.cn/anaconda/cloud/conda-forge/
    conda config --remove channels https://mirrors.tuna.tsinghua.edu.cn/anaconda/cloud/pytorch/
```

### 或者在pip的时候制定 源



```bash
pip install torch torchvision -i https://pypi.mirrors.ustc.edu.cn/simple/
```



将anaconda安装目录中的condabin添加到系统环境变量即可，

D:\anaconda\condabin ，
即可在命令行中直接使用conda命令

#### Linux下载anaconda并且安装

https://mirrors.tuna.tsinghua.edu.cn/anaconda/miniconda/

注意在此处添加环境变量

![image-20220111122117978](../../../../Lenovo/AppData/Roaming/Typora/typora-user-images/image-20220111122117978.png)

## 安装miniconda



```
wget -c https://repo.continuum.io/miniconda/Miniconda3-latest-Linux-x86_64.sh
```

 wget -c https://repo.continuum.io/miniconda/Miniconda3-latest-Linux-x86_64.sh

```bash
wget https://mirrors.tuna.tsinghua.edu.cn/miniconda/Miniconda3-latest-Linux-x86_64.sh
```

```
chmod +x Miniconda3-latest-Linux-x86_64.sh
```

 

```
./Miniconda-latest-Linux-x86_64.sh
```



## 安装anaconda

https://repo.anaconda.com/archive/Anaconda3-2021.11-Linux-x86_64.sh

```bash
wget -c https://repo.anaconda.com/archive/Anaconda3-2021.11-Linux-x86_64.sh
```

 

```
chmod +x https://repo.anaconda.com/archive/Anaconda3-2021.11-Linux-x86_64.sh
```

 

```
./https://repo.anaconda.com/archive/Anaconda3-2021.11-Linux-x86_64.sh
```



## conda命令使用指南

进入D:\Research_2021\Face\Pytorch-MobileFaceNet-master 所在文件夹使用命令行打开

2.1输入conda 命令有反应 说明1中添加环境变量成功

TDD 牛逼



### 新建虚拟环境  python38

```
conda create -n ckq_py38 python=3.8
```

conda create -n python3 python=3.6

```bash
conda create -n face python=3.6
conda create -n face python=3.6
```

2.2 新建后进入虚拟环境  python38

```bash
conda activate  python38
```

删除虚拟环境

```
conda remove -n XXX --all
```



![image-20220111122958423](../../../../Lenovo/AppData/Roaming/Typora/typora-user-images/image-20220111122958423.png)

pip 慢

```
pip install 库包名 -i http://pypi.douban.com/simple/ --trusted-host pypi.douban.com
```

2.3使用pip下载requirements2.txt中所需文件

升级pip 

```python
pip show pip
python -m pip install --upgrade pip
```

conda慢 -i 清华源

pip慢

```bash
pip install -i https://pypi.tuna.tsinghua.edu.cn/simple -r  requirements2.txt
```

2.4在所在D:\Research_2021\Face\Pytorch-MobileFaceNet-master文件夹下运行python模块

```bash
python infer.py temp/test.jpg
```

运行结果如下

![image-20220111123751252](../../../../Lenovo/AppData/Roaming/Typora/typora-user-images/image-20220111123751252.png)

人工智能模块可运行

2.5在该文件夹下使用如下命令获取python的位置记为位置一

```bash
conda info --envs
```

![image-20220111124145617](../../../../Lenovo/AppData/Roaming/Typora/typora-user-images/image-20220111124145617.png)

```bash
conda env remove -n tensorflow-2.7
```

在该文件夹下获取infer.py的位置记为位置二

删除虚拟环境

```bash
deactivate #如果需要删除当前环境的话
conda env remove -n tensorflow-2.7
```

![image-20220416120947153](../../../../Lenovo/AppData/Roaming/Typora/typora-user-images/image-20220416120947153.png)

![image-20220416121000641](../../../../Lenovo/AppData/Roaming/Typora/typora-user-images/image-20220416121000641.png)







## pip太慢的解决方法

## pip install -i https://pypi.tuna.tsinghua.edu.cn/simple -U sklean

![image-20220110205659513](../../../../Lenovo/AppData/Roaming/Typora/typora-user-images/image-20220110205659513.png)





https://blog.csdn.net/asdfgh0077/article/details/106079083/)

## 列表生成式子

https://www.cnblogs.com/ghostwu/p/8647343.html

## conda含义

```
conda info --envs 	
```

显示环境路径名称

conda新建环境

```bash
conda create -n face python=3.6
```

conda 删除环境

```bash
conda remove -n env-name --all 
```

conda列出所有包

[Linux下安装face_recognition库（人脸识别） - 简书 (jianshu.com)](https://www.jianshu.com/p/925229426619)

```
conda list
```

老师好，请问我能选择废弃我的期中成绩，直接用期末成绩覆盖期中占比吗？（相当于期中没来考）这样既不影响公平，我也保证我期末复习后能过。如果您这边同意的话我找助教登记一下。




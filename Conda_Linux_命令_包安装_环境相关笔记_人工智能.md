[TOC]

Gtlihub

Support for password authentication was removed on August 13, 2021. Please use a personal access token instead.



[Support for password authentication was removed on August 13, 2021. Please use a personal access ... - 简书 (jianshu.com)](https://www.jianshu.com/p/d5f2e04a332f)

```cpp
git remote set-url origin https://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@github.com/ckqqqq/TDD2.git/
```



## Django



## pycharm

使用正则表达式处理(替换) 

炒鸡牛逼的文本处理工具

一键去除所有注释

![image-20220613010829940](C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20220613010829940.png)

## 如何打开django文件

windows

## pycharm数据库

## Driver class 'org.sqlite.JDBC'not found Driver files are not downloaded.(moments ago)

[(57条消息) 问题：pycharm database查看db.sqlites文件提示：Driver class ‘org.sqlite.JDBC‘ not found_奔跑中的小猿的博客-CSDN博客](https://blog.csdn.net/weixin_42230348/article/details/108202185)

![image-20220531144322647](C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20220531144322647.png)

Lo

[(56条消息) 问题：在Ubantu系统下，输入ifconfig只有lo，没有eth0,(已解决)_大西瓜-PaulChan的博客-CSDN博客_ubuntu只有lo没有eth0](https://blog.csdn.net/qq562029186/article/details/74295659?spm=1001.2101.3001.6650.1&utm_medium=distribute.pc_relevant.none-task-blog-2~default~CTRLIST~default-1-74295659-blog-120395632.pc_relevant_default&depth_1-utm_source=distribute.pc_relevant.none-task-blog-2~default~CTRLIST~default-1-74295659-blog-120395632.pc_relevant_default&utm_relevant_index=2)

网络配置复原

log4j.properties

```bash
log4j.rootLogger=INFO, stdout
log4j.appender.stdout=org.apache.log4j.ConsoleAppender
log4j.appender.stdout.layout=org.apache.log4j.PatternLayout
log4j.appender.stdout.layout.ConversionPattern=%d %p [%c] - %m%n
log4j.append
er.logfile.File=target/spring.log
log4j.appender.logfile.layout=org.apache.log4j.PatternLayout
log4j.appender.logfile.layout.ConversionPattern=%d %p [%c] - %m%n
```

# linux常见命令

## 基本单词翻译

```
ls=list 
cd=change directory
cp=copy
rm=remove
cat=concatenate把事物联系到一起 建议用more
pwd=password 
ps=process status
df=disk free
du=disk usage
mkdir=make directory
rmdir=remove directory
su=switch user
chown=change owner 
chmod=change mode



-a =all 
-l =list
-f=force
-n=number
-u=user
-h=human-readable
-z=zip
-v=verbose 冗余的
-q -quiect
-r recursive 递归的



```

## 查询操作方式

### TLDR

TLDR是著名的Linux命令行手册开源项目，是英语Too Long Didn't Read（太长不看）的缩写，就是想反对冗长的man和help内容，建立一个简化的、社区驱动的手册集合。

- TLDR的GitHub地址：[tldr-pages/tldr](https://link.zhihu.com/?target=https%3A//github.com/tldr-pages/tldr)
- 命令查询 [tldr | simplified, community driven man pages (ostera.io)](https://tldr.ostera.io/ls)
- [ls命令 – 显示指定工作目录下的文件及属性信息 – Linux命令大全(手册) (linuxcool.com)](https://www.linuxcool.com/ls)

TLDR可以安装在Linux上，然后使用tldr  <commandname>就能快速查找，也有Web、Android 和 iOS 版本可以使用。





## .sh文件

-bash: ./print_assemble_code.sh: Permission denied

```bash
chmod 777 *.sh
```

## 文件操作

按下shift加ctrl键可以有条件全选

./print_function_assemble_code.sh

## Linux虚拟机gcc

```
gcc -o 中间文件名 .c文件
./ 可执行文件
```



## linux 虚拟机使用ssh

```bash
sudo apt-get openssh-server

```

![image-20220523192219647](C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20220523192219647.png)



```bash
ssh-keygen -R 192.168.174.128
```



输入命令：netstat -ano|findstr "8081查看指定端口



```bash
netstat -ano|findstr "8081"
```



## Docker





[Istio / 使用 Kubernetes 和 Istio 学习微服务](https://istio.io/latest/zh/docs/examples/microservices-istio/)



## 换源

```python
   conda config --add channels https://mirrors.tuna.tsinghua.edu.cn/anaconda/pkgs/main/
    conda config --add channels https://mirrors.tuna.tsinghua.edu.cn/anaconda/pkgs/free/
    conda config --add channels https://mirrors.tuna.tsinghua.edu.cn/anaconda/cloud/conda-forge/
    conda config --add channels https://mirrors.tuna.tsinghua.edu.cn/anaconda/cloud/pytorch/
```



```
   conda config --remove channels https://mirrors.tuna.tsinghua.edu.cn/anaconda/pkgs/main/
    conda config --remove channels https://mirrors.tuna.tsinghua.edu.cn/anaconda/pkgs/free/
    conda config --remove channels https://mirrors.tuna.tsinghua.edu.cn/anaconda/cloud/conda-forge/
    conda config --remove channels https://mirrors.tuna.tsinghua.edu.cn/anaconda/cloud/pytorch/
```



## Curl下载

```python
curl http://www.zhangblog.com/2019/06/16/hexo{04,05,06}/ -I  # 查看信息
curl下载网址
curl -O https://download.open-mpi.org/release/open-mpi/v4.0/openmpi-4.0.7.tar.gz
```

## tar解压

```bash
tar -xvf openmpi-4.0.0.tar.gz
```

## 多卡并行DIstributed

https://github.com/tczhangzhi/pytorch-distributed/blob/master/distributed.py

在主GPU上进行梯度计算和更新，再将参数给其他gpu,让他们反向传播

多卡并行DIstributed，这些进程在最开始的时候会保持一致，同时在更新模型的时候，梯度传播也是完全一致的，这样就可以保证任何一个GPU上面的模型参数就是完全一致的，所以这样就不会出现DataParallel那样的显存不均衡的问题。

## 多卡并行Horovod

Horovod 安装（pytorch可行）

https://github.com/horovod/horovod/blob/master/docs/install.rst

```bash
$ HOROVOD_WITH_PYTORCH=1 pip install horovod[pytorch]
```

失败hhhh

## 解决方法

报错一

```bash
Failed to build horovod
Installing collected packages: pyasn1, zipp, rsa, pyasn1-modules, oauthlib, multidict, frozenlist, cachetools, yarl, requests-oauthlib, pyparsing, importlib-metadata, google-auth, attrs, async-timeout, aiosignal, werkzeug, tensorboard-plugin-wit, tensorboard-data-server, pyDeprecate, protobuf, packaging, markdown, grpcio, google-auth-oauthlib, fsspec, aiohttp, absl-py, torchmetrics, tensorboard, pyyaml, future, pytorch-lightning, horovod
  Attempting uninstall: pyyaml
    Found existing installation: PyYAML 6.0
    Uninstalling PyYAML-6.0:
      Successfully uninstalled PyYAML-6.0
    Running setup.py install for horovod ... error

```



## 史上最全git操作

## Python语法请见算法md文件

![image-20220410204354081](C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20220410204354081.png)

## Git的使用教程

```bash
git add Article1
#加入暂存区域
git commit -m test
#
git push origin master
#正式提交
```

![image-20220402212344088](C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20220402212344088.png)

![image-20220402212416105](C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20220402212416105.png)

注意github新建仓库时尽量不要用模板

```bash
#github教程
echo "# CSDN" >> README.md
git init
#告诉git 开始对这些文件进行跟踪
git add README.md
#提交到暂时存储区，同时加上massage
git commit -m "first commit"
#这是一个改名操作，将当前分支名改名为main
git branch -M main
#这是手动的为你的远程仓库的地址在本地起一个别名origin
git remote add origin https://github.com/ckqqqq/CSDN.git
#-upstream 将本地的main中的流上传到远程的origin（github上的远程也将命名为main）
git push -u origin main

#git 设置全局email
git config --global user.email "邮箱"
git config --global user.name "名字"
#git 设置本地email
git config  user.email "邮箱"
git config  user.name "名字"

```

查看变更

```bash
#查看提交到占存区的记录
git log
通过git checkout命令，我们可以切换到某个快照。
git checkout c9053865e9dff393fd2f7a92a18f9bd7f2caa7fa
#通过git show命令，我们可以显示某个快照的所有代码变更。
git show c9053865e9dff393fd2f7a92a18f9bd7f2caa7fa
```

![image-20220710170758816](https://s2.loli.net/2022/07/10/5eCsxFmcRQXyAB3.png)

设置git为中文

![image-20220710170924814](https://s2.loli.net/2022/07/10/4hFiZ1cs5lGz86t.png)

```bash
git config --global core.quotepath false 
git config --global i18n.commitencoding utf-8
git config --global i18n.commitencoding utf-8
git config --global i18n.logoutputencoding utf-8
export LESSCHARSET=utf-8
https://blog.csdn.net/weixin_44797327/article/details/123715751
```

OpenSSL问题

![image-20220710171416538](../../AppData/Roaming/Typora/typora-user-images/image-20220710171416538.png)

```bash
#问题一
git config --global http.sslVerify "false"
#问题二
vpn有问题换fastgithub

```



```
echo "# SpringBoot-Vue-Mybatis-Mysql_list_view" >> README.md
git init
git add README.md
git commit -m "first commit"
git branch -M main
git remote add origin https://github.com/ckqqqq/SpringBoot-Vue-Mybatis-Mysql_list_view.git
git push -u origin main
```

### …or push an existing repository from the command line



```
git remote add origin https://github.com/ckqqqq/SpringBoot-Vue-Mybatis-Mysql_list_view.git
git branch -M main
git push -u origin main
```



```bash
fatal: unable to access 'https://github.com/ckqqqq/Springboot-Vue-Mybatis-Simple-List-Template.git/': OpenSSL SSL_read: Connection was reset, errno 10054

git config --global http.sslVerify "false"
```

![image-20220526143015890](C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20220526143015890.png)

git ssh

gitee合并

pull request 

```

```

[(52条消息) 史上最简单Git入门教程_孤单品尝寂寞的博客-CSDN博客_git入门](https://blog.csdn.net/u011134399/article/details/122979552)

```bash
#commit 的时候碰到问题，运行下面两个就好了，不用加--global
git commit -m "测试提交"
*** Please tell me who you are.
Run
  git config  user.email "you@example.com"
  git config  user.name "Your Name"

to set your account's default identity.
Omit --global to set the identity only in this repository.
#新建分支
git branch test
git checkout 分支


```

```bash
#查看git 提交
git log

```

```bash
#查看变化
git diff --staged -M
```

git创建公钥

```bash
ssh-keygen -t rsa -C "ckqqqq@bupt.edu.cn"
```

windows本机的公钥位置

```bash
C:\Users\Lenovo/.ssh/id_rsa.pub
```



```
ssh -T git@github.com
```

然后全部复制到github上就行了

```
ssh-rsa AAAAB3NzaC1yc2EAAAADAQABAAABgQCYPxH7+dG7Y+pbTAiEoyy48QbHLWVKF0GmRI95tMEB27dUug3r+Wim7zEj9NEAuS9WySVRE1TCUHE/xjYdjXXC9JTjAG4gTIlXM7wVB2NO8ti9gY/++nFbTnEov3TXR4Xz1x5a1/TVvlQps2Fiy75d9JoP0FMimXtV8+jnyOrfvbxgxQLPag8ZrSec0iVXh7feCxskb4BusvlBFI3afKsSlJb2+K8yzXmubAczq2Bk0jN+D80bmmjlcolZqwNxkJCL00Oi6X9NjYQBHFxxBQV5hNrDgcBODjgCIt1gViMVzQBGk1CCwZnAWbHtcjxkdOsIcfPrzNo9kqSHbvA4qQgbouGC66Fued61vBv0uEWKOPZ/wnw+pn0dx4mkU8Ut2spz89FBW+PvJf7jS3DdoK2mh3yPB5En67o2UmkKYsjBQmCxcTjIN3PWv/JFYJfpj/zPLjVCHd0Jl2E2vCosHIClg7M/WTH+dWaNqtr9w6zvZW9kXATdbcXtjYK0iO4iSgs= ckqqqq@bupt.edu.cn

```

![](C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20220522193218902.png)

## Pycharm各种操作  

### 快速选择多个按键

- **`Ctrl`** + **`Shift`** + **`Alt`** + **`j`**
- ![image-20220429144225683](C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20220429144225683.png)

### **pycharm 字体放大设置：**

①，File —> setting —> Keymap —>在搜寻框中输入：increase —> Increase Font Size（双击） —> 在弹出的对话框中选择Add Mouse [Shortcut](https://so.csdn.net/so/search?q=Shortcut&spm=1001.2101.3001.7020) 

**2，Pycharm 字体缩小设置 ：**

①，File —> setting —> Keymap —>在搜寻框中输入：decrease —>Decrease Font Size（双击）—> 在弹出的对话框中选择Add Mouse Shortcut 

## Pycharm 全局查找

Find则是在当前文件查找，快捷键为**Ctrl + F**。这两个个功能非常实用。

Find in Path的使用：
按快捷键Ctrl + Shift + F或从从菜单Edit->Find->Find in Path进入全局查找界面。
如下图所示，在Text to find输入要查找的内容，可以说某个字符串，或者某个变量，再点击Find按钮，查找结果会显示在下方。

## 史上最全pytcharm配置远程服务器教程_我真的太牛逼了、

注意这里的重点是不能有中文文件夹名

Invalidate Cache/  Restart (这个是更新缓存并且重启)

![image-20220429103755145](C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20220429103755145.png)

### pycharm设置-远程服务器

![image-20220429103936739](C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20220429103936739.png)

![image-20220429104009747](C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20220429104009747.png)

如果没有，点击三个点





```bash
/home/ld/KeqiChen_model/tmp
```

![image-20220429141525398](C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20220429141525398.png)



### Pycharm设置远程编译器

你要记得检查编译器，这里有一个点，就是下面的编译器，虽然他们名字一样，但是他们的最后编译路径是不一样的，他们的map的路径是不一样的，所以如果碰到路径问题，请新建一个编译器



![image-20220429141220627](C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20220429141220627.png)

建议这里打开Configuration

![image-20220429104354675](C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20220429104354675.png)

![image-20220429104625215](C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20220429104625215.png)

![image-20220429104713219](C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20220429104713219.png)

警告:这里是你远程编译器的位置

![image-20220429104914951](C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20220429104914951.png)

设置本地和远程的映射

注意这里不能有中文

![image-20220429105201586](C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20220429105201586.png)

新建完成

![image-20220429105332817](C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20220429105332817.png)

![image-20220429105926958](C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20220429105926958.png)

注意这里不能有中文



Successfully Connect

![image-20220429105531652](C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20220429105531652.png)

```bash
D:/amyprocess/remote_zicheng2
#local path
/home/ld/KeqiChen_model/model
#remote path
/home/ld/.conda/envs/cke_py38/bin/python
#remote interpreter
```

![image-20220429110047668](C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20220429110047668.png)

上面这个因为有中文，所有有bug

![image-20220429135435612](C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20220429135435612.png)

部署完成

debug 部署

![image-20220429135400718](C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20220429135400718.png)

打开资源管理器，设置自动上传

一是勾选Automatic Upload 

而是打开 Browse

![image-20220429110338700](C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20220429110338700.png)

注意这里如果有模型两个字会导致无法正常编译

![image-20220429110217718](C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20220429110217718.png)

![image-20220429145934797](C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20220429145934797.png)

![image-20220429145958051](C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20220429145958051.png)

、

## 远程调试

![image-20220429145907912](C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20220429145907912.png)

## 最后结果

![image-20220429135200762](C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20220429135200762.png)





### 退出test模式

方法2：
如果上述方法，只是临时解决，过段时间又是[pytest](https://so.csdn.net/so/search?q=pytest&spm=1001.2101.3001.7020)了
可以进入 File-settings-python integrated tools里面修改，选择unittest修改后记得应用一下
参考下图

![image-20220426214352621](C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20220426214352621.png)

```

```



Pycharm远程映射

```

```



## GPU问题，并行问题

[【ubuntu】torch.cuda.is_available()结果为false - 知乎 (zhihu.com)](https://zhuanlan.zhihu.com/p/344785624)

```python

import torch
print(torch.cuda.is_available)


```

![image-20220426205245822](C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20220426205245822.png)

![image-20220426205158416](C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20220426205158416.png)

![image-20220426205214131](C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20220426205214131.png)

## 查看CPU版本，查看CUDA 版本

```python
nvidia-smi
```

![image-20220426200824872](C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20220426200824872.png)

## 软件过程改进_TDD_

```python
#python manage runserver
python ./superlists/manage.py runserver
python function_test.py
python "functional_tests _unit2.py"
#git
mv "functional_tests_unit2.py" superlists/
cd superlists
git init
dir
echo "db.sqlite3" >>.gitignore
echo "geckodriver.log" >>.gitignore
git add .
git status 
```

![image-20220426082253462](C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20220426082253462.png)

看到一堆pyc文件，移出他们

![image-20220426082614005](C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20220426082614005.png)

```python
git rm -r --cached superlists/__pycache__
echo "__pycache__" >> .gitigore
echo "*.pyc" >> .gitignore
git status
git add .gitignore
git commit
```

![image-20220426082813165](C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20220426082813165.png)

### 功能测试扩展

![image-20220426083701805](C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20220426083701805.png)

```python
from selenium import webdriver
import unittest
class NewVistorTest(unittest.TestCase):#
    def setUp(self):
        self.browser=webdriver.Firefox()
    def tearDown(self):
        self.browser.quit()
    def test_can_start_a_list_and_retrieve_it_latter(self):
        self.browser.get("http://localhost:8000")
        self.assertIn("TO-DO",self.browser.title)
        self.fail('Finish Test')
if __name__=='__main__':
    unittest.main(warnings="ignore")

```

![image-20220426084420317](C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20220426084420317.png)

```python
git status
git diff
```

![image-20220426084553879](C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20220426084553879.png)



```
#查看不同
git difftool
#省流版
git diff --staged
```

![image-20220426085104660](C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20220426085104660.png)

### unit3简单主页的单元测

![image-20220426085331297](C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20220426085331297.png)

```
python manage.py startapp lists
#打开 superlists/lists/test.py
from django.test import TestCase

# Create your tests here.
class SmokeTest(TestCase):
    def test_bad_maths(self):
        self.assertEqual(1+1,3)
git status
git add lists
git diff --staged
git commit -m "ADD app from lists"

```



```python
#tests.py
from django.test import TestCase

# Create your tests here.
class SmokeTest(TestCase):
    def test_bad_maths(self):
        self.assertEqual(1+1,3)
```

```python
python manage.py test
```

![image-20220426090413749](C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20220426090413749.png)

```
git status
git add lists
git diff --staged
git commit -m "ADD app from test,failing unit test"
git commit -m "ADD app from test,failing unit test"
```

```python
#tests.py
from django.urls import resolve
from django.test import TestCase
from lists.views import home_page
class HomePageTest(TestCase):
    def test_root_url_resolve_to_home_page_view(self):
        found=resolve("/")#解析URL
        self.assertEqual(found.func,home_page)#网站的根目录应该有一个home——page网页
#views.py
from django.shortcuts import render
home_page=None
#urls.py#这里和老师不一样
from django.urls import path
from lists import views
urlpatterns = [
    path('',views.home_page,name='home'),
]#该表达式定义它应用于哪些URL，


```

![image-20220426093530850](C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20220426093530850.png)

```
git commit -am XXX

```



```python
#tests.py
from django.urls import resolve
from django.test import TestCase
from django.http import HttpRequest
from lists.views import home_page
class HomePageTest(TestCase):
    def test_root_url_resolve_to_home_page_view(self):
        found=resolve("/")#解析URL
        self.assertEqual(found.func,home_page)#网站的根目录应该有一个home——page网页
    def test_home_page_returns_correct_html(self):
        request=HttpRequest()
        response=home_page(request)
        html=response.content.decode('utf-8')
        self.assertTrue(html.startswith("<html>"))
        self.assertIn("<title>To-Do lists</title>",html)
        self.assertTrue(html.endswith("</html>"))
#Views.
from django.shortcuts import render
from django.http import HttpResponse
def home_page(request):
    return HttpResponse(r"<html><title>To-Do lists</title></html>")
# Create your views here.

```



## 方法论

如果虚拟机百般配置不行，建议直接remake最快

背熟linux命令，效率是一切之本！！！

教训：vscode类似notepad ，是一种文本读写工具而不是开发工具，

所以远程连接LINUX最好的方法就是Xshell+xftp(能用ide打开并保存，同时命令行运行)

回海南后重装VScode

## Markdown使用指南

表格可以直接黏贴到excel里面

回海南后还要写一下自己的typora图床



### Openstreetmap教程

如何获得葡萄牙数据？

这个是欧洲各国数据

[Get all POI's for a city - OSM Help (openstreetmap.org)](https://help.openstreetmap.org/questions/43759/get-all-pois-for-a-city)

[Index of /europe (geofabrik.de)](http://download.geofabrik.de/europe/)

[Index of /europe (geofabrik.de)](http://download.geofabrik.de/europe/)

[如何用osmfilter和其他任何标签信息一起滤除所有设施？ - 码客 (oomake.com)](https://oomake.com/question/8219697)

## Osmosis运行教程

```bash
sudo apt install osmosis
这样竟然也能装
```

[Osmosis - OpenStreetMap Wiki](https://wiki.openstreetmap.org/wiki/Osmosis#Linux)

## chmod 命令含义

chmod是添加更改权限命令
a是指所有的用户组，包括root用户组，文件拥有者的用户组，还有其他用户组。
+x是指添加执行权限。


+x是执行权限，+r是阅读权限，+w是写入权限

## Ubuntu不能用git怎么办

#### 修改host

1 



```
sudo vim /etc/hosts
 dlcdn.apache.org
```

2

在里面加入

ip在这个网站里面查

这里是中国的ip

["www.github.com"A记录/cname检测结果\--Dns查询\|dns查询\--站长工具
(chinaz.com)](https://tool.chinaz.com/dns?type=1&host=www.github.com&ip=)

![image-20220330123509030](C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20220330123509030.png)

3 不过即使这样也ping不通，但是可以git clone了，这本质是一种代理

4 

```bash
sudo /etc/init.d/networking restart
```

[(66条消息) sudo: command not found 的解决方法_ByteSaid的博客-CSDN博客](https://blog.csdn.net/hello_1995/article/details/109222650)

![image-20220330125244925](C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20220330125244925.png)



### Pandoc（windows）使用orz

Pandoc是一个文档转换工具他可以将比如word类型转换成Latex类型或者其他奇奇怪怪的类型

[Convert a Word Document into MD (github.com)](https://gist.github.com/jesperronn/ff5764274b3642bc7f2f#file-docx2md-sh)

不过看他的教程记得要看最新版的

比如将docx 类型转换为带有图片的md类型

![image-20220330104529428](C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20220330104529428.png)

![image-20220330104739965](C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20220330104739965.png)



在文件夹下面生成一个装有图片的文档还有.md文件,更牛逼的是他们使用的是相对路径

当然表格的转换有点问题，你可以继续看看教程，可以设置标准word之类的，牛逼！

好的-reference.docx

https://github.com/fractaledmind/pandoc_docx_template/blob/master/academic_test.docx

Pandoc **在本机上一些有用的命令**

```bash
pandoc -f docx -t markdown  --extract-media="./csdn_hadoop_install" -o "hadoop安装.md" "hadoop_伪分布式安装.docx" --lua-filter="no_h_w.lua"
#这个命令就不会产生height和width

pandoc -f docx -t markdown  --extract-media="./openstack文档的图片" -o "openstack安装和github换源.md" "陈可淇_2019211955_实验一.docx"
pandoc -f docx -t markdown  --extract-media="./openstack文档的图片" -o "openstack安装和github换源.md" "陈可淇_2019211955_实验一.docx"
pandoc -t docx "D:\Cache\PictureCache\在linux上安装openstack.md" --reference-doc="D:\Cache\PictureCache\custom-reference.docx" -o "test.docx"
```



### md 转word

```bash

pandoc -o custom-reference.docx --print-default-data-file reference.docx
```

## 如何使用Pandoc将文档转化为docx

typora入门

[Typora入门：全网最全教程 | typora中文网](https://www.typora.net/1249.html)

使用markdown写ppt

见微信

pandoc 写论文 latex

https://github.com/Wandmalfarbe/pandoc-latex-template

pandoc 图标引用

https://github.com/tomduck/pandoc-fignos#usage

一个简短的latex介绍

https://liam.page/2014/09/08/latex-introduction/

### Markdown Syntax

The cross-referencing syntax used by pandoc-fignos was developed in [pandoc Issue #813](https://github.com/jgm/pandoc/issues/813) -- see [this post](https://github.com/jgm/pandoc/issues/813#issuecomment-70423503) by [@scaramouche1](https://github.com/scaramouche1).

To mark a figure for numbering, add an identifier to its attributes:

```
![Caption.](image.png){#fig:id}
```

The prefix `#fig:` is required. `id` should be replaced with a unique string composed of letters, numbers, dashes and underscores.  If `id` is omitted then the figure will be numbered but unreferenceable.  Alternatively, [reference link](http://pandoc.org/MANUAL.html#reference-links) attributes may be used.

To reference the figure, use

```
@fig:id
```

or

```
{@fig:id}
```

Curly braces protect a reference and are stripped from the output.

Demonstration: Processing [demo.md](https://raw.githubusercontent.com/tomduck/pandoc-fignos/master/demos/demo.md) with pandoc + pandoc-fignos gives numbered figures and references in [pdf](https://raw.githack.com/tomduck/pandoc-fignos/demos/demo.pdf), [tex](https://raw.githack.com/tomduck/pandoc-fignos/demos/demo.tex), [html](https://raw.githack.com/tomduck/pandoc-fignos/demos/demo.html), [epub](https://raw.githack.com/tomduck/pandoc-fignos/demos/demo.epub), [docx](https://raw.githack.com/tomduck/pandoc-fignos/demos/demo.docx) and other formats.

[![Wall.E](https://pica.zhimg.com/v2-09cf93125231c8f207db80351e5e798f_xs.jpg?source=172ae18b)](https://www.zhihu.com/people/yang-zhi-hong)

[Wall.E](https://www.zhihu.com/people/yang-zhi-hong)

21 人赞同了该文章



## Pandoc

[Pandoc](https://link.zhihu.com/?target=http%3A//pandoc.org/)是一个文档转换工具，支持docx、markdown、html、pdf、txt等等文件格式的互相转化，作者[John MacFarlane](https://link.zhihu.com/?target=http%3A//johnmacfarlane.net/)是美国加州大学伯克利分校的哲学教授。

### 用法实例



文章[如何使用Pandoc将文档转化为docx - 知乎 (zhihu.com)](https://zhuanlan.zhihu.com/p/49530707)

### markdown转docx

```bash
pandoc demo-math.md -o demo-math.docx
```

将名为`demo-math.md`的文件转化为`demo-math.docx`的word文档。

### 转docx并指定样式

```bash
pandoc -s m.md -S --reference-docx reference.docx -o m.docx
```

将名为`m.md`的文件转化为`m.docx`的word文档，同时使用reference.docx中的样式作为模板，这在一定程度上实现了word创作时的内容和表现分离。

### 转docx并自动生成参考文献

```bash
pandoc --filter pandoc-citeproc --bibliography=myref.bib --csl=chinese-gb7714-2005-numeric.csl demo-citation.md -o demo-citation.docx
```

将名为`demo-citation.md`的文件转化为`demo-citation.docx`的word文档，同时自动生成参考文献。参考文献格式由`csl`文件指定，参考文献内容在`myref.bib`中。

其中markdown文件中写入参考文献的方式为：

```text
[@王国成2017从]
```

### 转docx时实现图文交叉引用

```bash
pandoc --filter pandoc-fignos demo-figref.md -o demo-figref.docx
```

将名为`demo-figref.md`的文件转化为`demo-figref.docx`的word文档，同时自动生成图表编号。其中`pandoc-fignos`需要提前使用pip工具安装（`pip install pandoc-fignos`）

markdown文件要使用自动图表编号，首先在文件头部写入如下信息：

```text
---
fignos-cleveref: On
fignos-plus-name: 图
...
```

然后再在图表和引用处标记：

```text
大数据的3V特性如{@fig:bigdata3v}所示

![大数据的3V特性](assets/demo-a5a137d9.png){#fig:bigdata3v}
```

### 参考资料

1. [如何用Markdown写论文？](https://zhuanlan.zhihu.com/p/31690364)
2. [pandoc-fignos](https://link.zhihu.com/?target=https%3A//github.com/tomduck/pandoc-fignos)
3. [pandoc-citeproc](https://link.zhihu.com/?target=https%3A//hackage.haskell.org/package/pandoc-citeproc)
4. [Pandoc手册](https://link.zhihu.com/?target=http%3A//pandoc.org/MANUAL.html)

发布于 2018-11-13 13:21

### Ubuntu20.04安装apache2浏览器

sudo  apt-get  install  apache2

```
#碰到端口占用问题
netstat -lnp|grep 80
netstat -lnp|grep 8080
```

[W3M - 一款终端浏览器 | linux软件 (linux265.com)](https://linux265.com/soft/3888.html)

按 q退出

## purge remove 彻底删除



```
sudo apt-get --purge remove XXX --purge
```



### su: Authentication failure 错误

su命令不能切换root，提示su: Authentication failure，只要你sudo passwd root过一次之后，下次再su的时候只要输入密码就可以成功登录了。

## 轨迹预测方向

Py

Linux 换源 apt

Windows添加环境变量

你可以在系统变量里面shishi



## 安装hadoop

![image-20220325123917296](C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20220325123917296.png)

java8位置



## Nohup

/home/ypl/anaconda3/envs/CKQPY38/bin

[(41条消息) 使用nohup运行python文件报错：Import error: No module named XXX等_lumia-.-的博客-CSDN博客](https://blog.csdn.net/lumiyaa/article/details/80515393)

[Windows使用cmd命令行中查看、修改、删除与添加环境变量 - springsnow - 博客园 (cnblogs.com)](https://www.cnblogs.com/springsnow/p/12610417.html)

输入which python，得到当前默认使用的python路径：



这时，只要指定python版本来运行nohup文件即可：

也就是：

nohup python main.py > log.txt2>&1 &。

```javascript
nohup python -u main.py  > flush.log 2>&1 &
nohup /home/ypl/anaconda3/envs/CKQPY38/bin/python3 locate.py > log.txt2>&1 &。
nohup /home/ypl/anaconda3/envs/CKQPY38/bin/python3 -u locate.py  > flush.log 2>&1 &
    
```

**其中，1代表标准输出，2代表标准错误输出，2>&1 是将标准错误输出重定向到标准输出，也就是将标准输出和标准错误输出都输出到log.txt文件中，最后的&将程序变为后台守护进程，这样运行的程序就不会随着终端的挂起而停止。**

版权声明：本文为CSDN博主「lumia-.-」的原创文章，遵循CC 4.0 BY-SA版权协议，转载请附上原文出处链接及本声明。
原文链接：https://blog.csdn.net/lumiyaa/article/details/80515393



https://zhuanlan.zhihu.com/p/97012199)

### 在windows中运行多个python程序（bat批量处理）

运行python程序前面要加satrt

```bash
@echo off
@echo begin
pause

start D:\TOOL\Anaconda\Anaconda3\envs\py38_gpu\python.exe locate.py 3.csv
pause
```



```bash
#忘记进程号z
(base) ypl@liya-FitServer-G4460-V5:~/KeqiChen/Porto_poi$ ps fx
  PID TTY      STAT   TIME COMMAND
72507 ?        S      0:00 sshd: ypl@pts/1
72508 pts/1    Ss     0:00  \_ -bash
 1674 pts/1    R+     0:00      \_ ps fx
71025 ?        S      0:01 sshd: ypl@notty
71026 ?        Ss     0:00  \_ bash
71071 ?        S      0:00      \_ sh /home/ypl/.vscode-server/bin/dfd34e8260c270da74b5c2d86d61aee4b6d56977/bin/code-server --start-serv
71081 ?        Sl     0:30      |   \_ /home/ypl/.vscode-server/bin/dfd34e8260c270da74b5c2d86d61aee4b6d56977/node /home/ypl/.vscode-serv
71119 ?        Sl     0:05      |       \_ /home/ypl/.vscode-server/bin/dfd34e8260c270da74b5c2d86d61aee4b6d56977/node /home/ypl/.vscode-
71428 pts/0    Ss+    0:00      |       |   \_ /bin/bash
71849 pts/0    Tl     0:02      |       |       \_ python test2.py
71161 ?        Sl     0:48      |       \_ /home/ypl/.vscode-server/bin/dfd34e8260c270da74b5c2d86d61aee4b6d56977/node /home/ypl/.vscode-
71320 ?        Sl     1:12      |       |   \_ /home/ypl/.vscode-server/bin/dfd34e8260c270da74b5c2d86d61aee4b6d56977/node /home/ypl/.vsc
71735 ?        Sl     0:00      |       |   \_ /home/ypl/.vscode-server/bin/dfd34e8260c270da74b5c2d86d61aee4b6d56977/node /home/ypl/.vsc
71167 ?        Sl     0:06      |       \_ /home/ypl/.vscode-server/bin/dfd34e8260c270da74b5c2d86d61aee4b6d56977/node /home/ypl/.vscode-
 1254 ?        S      0:00      \_ sleep 180
58315 ?        S      0:00 python -u get_proto_poi.py
64219 ?        Ss     0:00 /lib/systemd/systemd --user
64220 ?        S      0:00  \_ (sd-pam)

```



### C盘满了怎么办



Windows使用

### 第一定律，没事不要乱杀进程

第二定律，最好使用conda的pip

D盘这个样子

![image-20220410132134798](C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20220410132134798.png)

![image-20220410132642678](C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20220410132642678.png)



牛逼666

![image-20220410132609370](C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20220410132609370.png)

你的硬盘里竟然有100个G的虚拟机hhhh

https://blog.csdn.net/weixin_39558804/article/details/111793226

bash

```bash
mklink /j "C盘的路径“”D盘的路径”
```

C:\Users\Lenovo>mklink /j "C:\Program Files\Docker" "D:\TOOL\Docker\Program Files\Docker"
拒绝访问。

guan



版权声明：本文为CSDN博主「Claroja」的原创文章，遵循CC 4.0 BY-SA版权协议，转载请附上原文出处链接及本声明。
原文链接：https://blog.csdn.net/claroja/article/details/65447860

## 使用三原则 

### 1 要在chenkeqi文件夹下使用！，不能动别人的文件夹里面的任何数据。

### 2 不要使用任何的rm命令，如果想删除 文件夹 请将打算删除的文件mv 到 trash_bin文件夹，我会定期删除。

### 3 移动，新建，修改包等操作前记得在咱们qq群里说一声，一起操作均基于不影响其他用户使用为前提，linux系统操作不熟悉在QQ群里问一下就行，大家的问题应该也有人碰到过



![image-20220127165048628](C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20220127165048628.png)

##  LinuxBash

### VIM

显示行号

## **1 临时显示行号**

如果只是临时显示vim的行号，只须按ESC键退出编辑内容模式，输入“：set number”后按回车键，就可以显示行号了。行号显示只是暂时的，退出vim后再次打开vim就不显示行号了。

![img](https://ask.qcloudimg.com/http-save/1022634/pq3l7t4iyt.jpeg?imageView2/2/w/1620)

## **2 永久显示行号**

如果想让vim永久显示行号，则需要修改vim配置文件vimrc。如果没有此文件可以创建一个。在启动vim时，当前用户根目录下的vimrc文件会被自动读取，因此一般在当前用户的根目录下创建vimrc文件，即使用下面的命令：  

![img](https://ask.qcloudimg.com/http-save/1022634/34qrmgc1uj.jpeg?imageView2/2/w/1620)

在打开的vimrc文件中最后一行输入：set number ，然后保存退出。再次用vim打开文件时，就会显示行号了。



删除行

```
dd
```

**删除行**

在Vim中删除一行的命令是dd。

以下是删除行的分步说明：

1、按Esc键进入正常模式。

2、将光标放在要删除的行上。

3、键入dd并按Enter键以删除该行。

注：多次按dd将删除多行。

参考：[dd命令_Linux dd命令使用详解：复制文件并对原文件的内容进行转换和格式化处理](https://ywnz.com/linux/dd/)。

 

**删除多行**

要一次删除多行，请在dd命令前添加要删除的行数，例如，要删除五行，请执行以下操作：

1、按Esc键进入正常模式。

2、将光标放在要删除的第一行上。

3、键入5dd并按Enter键以删除接下来的五行。

 

**删除行范围**

删除一系列行的语法如下：

:[start],[end]d

例如，要删除从3到5的行，您可以执行以下操作：

1、按Esc键进入正常模式。

2、输入:3,5d，然后按Enter键以删除行。

您还可以使用以下字符来指定范围：

.（点）-当前行。

$-最后一行。

%-所有行。

这里有一些例子：

:.,$d-从当前行到文件末尾。

:.,1d-从当前行到文件开头。

10,$d-从第十行到文件末尾。

### 如果对linux命令不熟悉，可以使用以下教程，别用rm命令！！！！

https://blog.csdn.net/qq_23329167/article/details/83856430

以下为使用命令行模式进入系统的方法

打开webvpn，将搜索框调整为ssh，输入以下ip和端口

IP:

10.99.4.35

端口

10876

![image-20220127174619905](C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20220127174619905.png)

跳转后输入

**账号 chenkeqi**

**密码 chenkeqi**

![image-20220127174740784](C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20220127174740784.png)



uname 命令 uname -a 命令可以直接显示 Linux 系统架构的命令,几乎...



## 进入命令行后

#### 快速进入轨迹预测文件夹

```bash
cd /devdata/chenkeqi/trace_prediction
```

#### 各个命令含义

输入命令，作用了解空间

```bash
df -h
```

进入到这个还有1.8T的空间

![image-20220127173609553](C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20220127173609553.png)

```bash
cd /devdata
ls
```

其他文件夹是别人的数据，千万不要进错了

![](C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20220127173758127.png)

进入chenkeqi文件夹

```bash
cd chenkeqi
ls
```

下面的三个文件夹含义

![image-20220127173856367](C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20220127173856367.png)

NER :**命名实体识别文件夹 先别管**

trace_prediction文件夹：**存储有我们组的所有代码和模型，大家如果有需要共享的文件向向里面放置**

trash_bin文件夹：**是垃圾箱文件夹，如果打算删除任何文件使用以下命令，不要用rm！**

```bash
mv 要删除的文件夹名字 /devdata/chenkeqi/trash_bin
```

## 激活python环境（anaconda3）

**首先添加路径，添加后才能在命令行使用conda**

是这个

```bash
export PATH=/devdata/anaconda3/bin:$PATH
```

使用命令查看anaconda中的虚拟python环境

```bash
conda info --envs
```

![image-20220127175116403](C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20220127175116403.png)

当前环境介绍



![image-20220127175254495](C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20220127175254495.png)

base 环境

尽量用下面两个环境

base和XiaChenjin尽量不要使用

pytorch 环境 python 版本3.75 有kearas TF pytorch

tensorflow环境 python版本3.69 只有TF&Kearas 

可以install包，尽量不要删包

**激活某个环境，注意和平常用的命令不同**

```bash
source activate 要激活的环境名
```

![image-20220127175613175](C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20220127175613175.png)

conda的用法可以百度，conda类似针对某个python版本的虚拟机

**编译某个模型的方法**

```
python XXXX.py 参数 
```







## JAVA文件讀寫

注意不要覆蓋之前的輸入





作者：ShanSly
链接：https://www.jianshu.com/p/0534043b4471
来源：简书
著作权归作者所有。商业转载请联系作者获得授权，非商业转载请注明出处。



## Pycharm使用指南

### 同名文件警告

警告在命名pycharm文件时，不要命名为re.py

## 区别Anaconda和miniconda

###### 1、Anaconda：

①Anaconda是一个开源的Python发行版本，包含了conda、python等180多个科学包及其依赖项。
 ②相当于一堆科学计算常用包，重量级

###### 2、Miniconda：

①通过以上对Anaconda的介绍，我们了解到Anaconda的数据包和和安装包都很大，所以如果我们需要较少的时间去做 这样的事情，就是Miniconda的登场！
 ②Miniconda是最小的conda安装环境，相当于conda+python+pip，轻量级

## Anaconda安装指南

#### 1 Windows下载anaconda并且安装

https://mirrors.tuna.tsinghua.edu.cn/anaconda/miniconda/

注意在此处添加环境变量

![image-20220111122117978](C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20220111122117978.png)

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

![image-20220111122958423](C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20220111122958423.png)

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

![image-20220111123751252](C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20220111123751252.png)

人工智能模块可运行

2.5在该文件夹下使用如下命令获取python的位置记为位置一

```bash
conda info --envs
```

![image-20220111124145617](C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20220111124145617.png)

```bash
conda env remove -n tensorflow-2.7
```

在该文件夹下获取infer.py的位置记为位置二

删除虚拟环境

```bash
deactivate #如果需要删除当前环境的话
conda env remove -n tensorflow-2.7
```

![image-20220416120947153](C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20220416120947153.png)

![image-20220416121000641](C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20220416121000641.png)







## pip太慢的解决方法

## pip install -i https://pypi.tuna.tsinghua.edu.cn/simple -U sklean

![image-20220110205659513](C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20220110205659513.png)





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

## DOTNET

.Net框架下列出.net 的所有可运行版本





```net
dotnet Mydll.dll  列出所有路径
dotnet --list-runtimes 列出所有运行中的版本
```



## NP

squeeze 去掉维度的函数

`np.squeeze`这个函数的作用是去掉矩阵里维度为1的维度。

例：(1, 300)的矩阵经由`np.squeeze`处理后变成300; (200, 1, 300)的矩阵经由`np.squeeze`处理后变成(200, 300)。

## 切片

切片的本质为从A到B

```
input = input_chars[:]
```

[切片 - 廖雪峰的官方网站 (liaoxuefeng.com)](https://www.liaoxuefeng.com/wiki/1016959663602400/1017269965565856)![image-20211122012723684](C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20211122012723684.png)



![image-20211122001847947](C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20211122001847947.png)



杨老师您好，我是您大三编译原理课程的学生。请问您能降低期中考试的分数占比吗，下调一个比例，比如从20%下调到10%这样？我问了一下身边的人，他们普遍反映期中考试难度和题量太大了，很多人是因为没掌握考试技巧只有三四十分，大家的信心都很受打击，影响了大家备考期末考试的状态。甚至还有人算了占比后直接放弃期末了。

​         您可以将降低后的分数比例移至期末考，一来大家也能恢复一点信心，二来我相信同学们经历这一次大题量大难度的期中考试后，一定会以200%的精力优先复习编译原理的，这样期末大家的通过率也就会高。

​        杨老师，原本这次期中考试后，我身边大多数同学开始重视并编译原理课程了，但是得知出分和占比后又有好多人深受打击，陷入了自我怀疑中。许多同学都希望您能减低本次期中的比例，我们向您保证：期末考试我们绝对会拼命复习，争取高分的。

## Linux环境 VMtool 网络

VMtool

1604版本看DVD哪里

![image-20211205125327874](C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20211205125327874.png)

tar -zxvf +tab键

命令：tar -zcvf 打包压缩后的文件名 要打包的文件
其中：z：调用gzip压缩命令进行压缩
 c：打包文件
 v：显示运行过程
 f：指定文件名

命令：tar [-zxvf] 压缩文件   
其中：x：代表解压
示例：将/usr/tmp 下的ab.tar解压到当前目录下

## 安裝中文輸入法

[(33条消息) ubuntu16.04 安装谷歌拼音输入法_Sweet Baby，甜宝-CSDN博客](https://blog.csdn.net/u013132035/article/details/83987933)

##  LinuxBash

### 好用的教程

https://blog.csdn.net/qq_23329167/article/details/83856430

gedit linux上的word编辑器

### linux命令快捷键

输入前三个字符tab自动补全

ctrl +alt +t shell窗口

### Linux常用命令

### 创建目录

```
mkdir   aaa
```

​       在当前目录下创建一个名为aaa的目录
mkdir   /usr/aaa   在指定目录下创建一个名为aaa的目录

### 新建文件

```
 touch  aa.txt
```



#### MV改名或者移动

```bash
mv 路径一XXX  路径二XXX
```

mv test.txt wbk.txt

将文件test.txt重命名为wbk.txt：

```
 mv test.txt wbk.txt
```



-b ：若需覆盖文件，则覆盖前先行备份。 
-f ：force 强制的意思，如果目标文件已经存在，不会询问而直接覆盖；
-i ：若目标文件 (destination) 已经存在时，就会询问是否覆盖！
-u ：若目标文件已经存在，且 source 比较新，才会更新(update)
  -t ： --target-directory=DIRECTORY move all SOURCE arguments into DIRECTORY，即指定mv的目标目录，该选项适用于移动多个源文件到一个目录的情况，此时目标目录在前，源文件在后。

4．命令实例：

#### CP复制或者备份



```bash
cp xxx xxx.backup
```

#### 删除包

```bash
sudo apt remove g++
```

#### 查看端口号占用

```bash
netstat -anp |grep XXX
查看所有
netstat -nultp
```



#### 安装包

```bash
sudo apt-get install g++
```

## 大数据笔记

##### 安装java

/

```
我的java地址
sudo apt install openjdk-8-jdk
/usr/lib/jvm/java-8-openjdk-amd64/jre/bin/java
java home地址
/usr/lib/jvm/java-8-openjdk-amd64
```

寻找安装路径、

```bash
which java
看看这是否是个软连接，找出这个软连接指向的路径
ls -i 地址
ls -i 指向的地址
```

配置java 环境

![image-20220318120426680](C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20220318120426680.png)



#### 安装hadoop 2.1

[Apache Hadoop](https://hadoop.apache.org/release/2.10.1.html)

```
tar -zxvf hadoop-3.2.2.tar.gz
```

```
HADOOP_HOME=lXXX/hadoop
export PATH=$PATH:$HADOOP_HOME/bin:$HADOOP_HOME/sbin
```

我的路径

**/etc/profile**

```
/Desktop/Hadoop_tar/hadoop-2.10.1 
```

```bash
PATH=$PATH:$HOME/bin
export JAVA_HOME=/usr/lib/jvm/java-8-openjdk-amd64
export HADOOP_HOME=/Desktop/Hadoop_tar/hadoop-2.10.1 
export PATH=$PATH:$JAVA_HOME/bin:$HADOOP_HOME/bin
export CLASSPATH=$JAVA_HOME/lib
```

![image-20220318122841121](C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20220318122841121.png)



![image-20220318133332032](C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20220318133332032.png)

## 计网笔记 chmod

#### 功能：改变文件权限

Chmod 代表change model

```c++
sudo chmod 777 ./client
```

r表是读 (Read) 、w表示写 (Write) 、x表示执行 (execute)

读、写、运行三项权限可以用数字表示，就是r=4,w=2,x=1，777就是rwxrwxrwx，意思是该登录用户（可以用命令id查看）、他所在的组和其他人都有最高权限。

## 计网笔记 IPtable

#### 功能：sudo iptable ：对Iptable进行删改工作。

可以在IPtable中增加过滤规则，对来自源IP的包一律丢弃

可嵌入到C中，使用Sytem（"XX"）执行

```c++
sudo iptable -A/-D input -s IP DROP
```

-A=ADD -D=delete

-s=source 



登录用户（可以用命令id查看）、他所在的组和其他人都有最高权限。

​                               ![image-20211217214239333](C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20211217214239333.png)

### 计网路由实验

#### 编译运行

```bash
g++ -std=gnu++1z *.cpp -o dv-routing
```



#### 打印路由表

```ini
./dv-routing nodeA ./config/nodeaddr.txt ./config/topology.txt
```

./dv-routing nodeB ./config/nodeaddr.txt ./config/topology.txt

./dv-routing nodeC ./config/nodeaddr.txt ./config/topology.txt

./dv-routing nodeD ./config/nodeaddr.txt ./config/topology.txt

./dv-routing nodeE ./config/nodeaddr.txt ./config/topology.txt

无穷计数和毒性反转问题

毒路由和毒性反转是有区别的，毒路由是讲实话，链路断了之后就给所有邻居发，毒性反转是讲的假话，是源路由如果经过中间路由到达目的路由的情况下，会告诉中间路由我和目的路由是不可达的，可能他和目的路由是可达的但是费用较高而已，这样可以避免链路费用突然上升这种坏消息导致的路由循环。

![image-20211204223524451](C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20211204223524451.png)

![image-20211204222029239](C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20211204222029239.png)

![image-20211204222057839](C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20211204222057839.png)



![image-20211204222124071](C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20211204222124071.png)

作者：徐小德
链接：https://www.zhihu.com/question/39319653/answer/365452121
来源：知乎
著作权归作者所有。商业转载请联系作者获得授权，非商业转载请注明出处。

### g++ fatal error

没有进入正确的文件

## Chmod

### *sudo* /etc/*init.d*/networking restart

```
sudo /etc/init.d/networking restart
```

## 启动ssh服务

```bash
sudo /etc/init.d/ssh start
 /etc/init.d/ssh restart
sudo gedit /etc/ssh/sshd_config #配置文件

service ssh start
```

如果没有

记得改为桥接模式

### 安装

```bash
sudo apt-get install openssh-server
```

### 删除整个ssh

```bash

sudo stop ssh
stop: Unable to connect to Upstart: Failed to connect to socket /com/ubuntu/upstart: Connection refused
qiker@ubuntu:~ $ ps -e|grep ssh
 14766 ?        00:00:00 sshd
qiker@ubuntu:~ $ kill 14766
bash: kill: (14766) - Operation not permitted
qiker@ubuntu:~ $ ls

sudo apt-get --purge remove openssh-server --purge
#删光光
```

#### 免密登录（阿里云成功）

base) root@iZ8vbhsfhga8yj95cx1410Z:

```bash
~/.ssh
ssh-keygen -t rsa -P ""
cat id_rsa.pub >> authorized_keys
#如果不行换台虚拟机
ssh localhost
```

##  sshd_config 配置文件 

/etc/ssh/sshd_config

### 文件API含义



```

```

```bash
Port 22
   “Port”设置sshd监听的端口号。

ListenAddress 192.168.1.1
   “ListenAddress”设置sshd服务器绑定的IP地址。

HostKey /etc/ssh/ssh_host_key
	“HostKey”设置包含计算机私人密匙的文件。
ServerKeyBits 1024
     “ServerKeyBits” #定义服务器密匙的位数。

LoginGraceTime 600
     “LoginGraceTime” #设置如果用户不能成功登录，在切断连接之前服务器需要等待的时间（以秒为单位）。

KeyRegenerationInterval 3600
    “KeyRegenerationInterval”#设置在多少秒之后自动重新生成服务器的密匙（如果使用密匙）。重新生成密匙是为了防止用盗用的密匙解密被截获的信息。



PermitRootLogin no
   “PermitRootLogin”#####设置root能不能用ssh登录。这个选项一定不要设成“yes”。

IgnoreRhosts yes
   “IgnoreRhosts”#设置验证的时候是否使用“rhosts”和“shosts”文件。

IgnoreUserKnownHosts yes
    “IgnoreUserKnownHosts”#设置ssh daemon是否在进行RhostsRSAAuthentication安全验证的时候忽略用户的“$HOME/.ssh/known_hosts”

StrictModes yes：
     “StrictModes”#设置ssh在接收登录请求之前是否检查用户家目录和rhosts文件的权限和所有权。这通常是必要的，因为新手经常会把自己的目录和文件设成任何人都有写权限。

X11Forwarding no
      “X11Forwarding”#设置是否允许X11转发。

PrintMotd yes
      “PrintMotd”#设置sshd是否在用户登录的时候显示“/etc/motd”中的信息。

SyslogFacility AUTH
      “SyslogFacility”#设置在记录来自sshd的消息的时候，是否给出“facility code”。

LogLevel INFO
      “LogLevel”设置记录sshd日志消息的层次。INFO是一个好的选择。查看sshd的man帮助页，已获取更多的信息。

RhostsAuthentication no
     “RhostsAuthentication”设置只用rhosts或“/etc/hosts.equiv”进行安全验证是否已经足够了。

RhostsRSAAuthentication no
     “RhostsRSA”#设置是否允许用rhosts或“/etc/hosts.equiv”加上RSA进行安全验证。

RSAAuthentication yes
      “RSAAuthentication”#设置是否允许只有RSA安全验证。

PasswordAuthentication yes
      “PasswordAuthentication”#设置是否允许口令验证。

PermitEmptyPasswords no
      “PermitEmptyPasswords”########设置是否允许用口令为空的帐号登录。

AllowUsers admin

记得从桥接模式改回来才能用remote ssh

```

![image-20211215202154905](C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20211215202154905.png)

#### 启动网络服务

service network start

service ssh status

#### ip 修改端口号

vim /etc/ssh/sshd_config#

/etc/ssh/sshd_config start

####  ip 查看端口号命令

ss -antpl

### Vscode

![image-20211205125943415](C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20211205125943415.png)

添加直接加

Open Configuration file也行

![image-20211205130043718](C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20211205130043718.png)

### 指纹概念理解

指纹（fingerprint）：唯一标识一台主机。

```shell
当你第一次ssh连接一台服务器主机的时候，服务器返回了指纹，让你确认指纹是否正确，如果确认无误并且加入到 know_hosts 里，主机ip和指纹一一对应。
之后再次访问主机的时候，会对比服务器返回的指纹和 know_hosts里的是否一致，一致就顺利连接，不一致就警告⚠️中间人攻击。
```

### 公钥和私钥概念理解

这个私钥和公钥到底是什么概念？

简单说，公钥就是你的银行帐户，这个可能别人也知道，但只有手上有信用卡或是存折才能有资格去试帐户密码。所以这个信用卡和存折就是你的私钥。所以这个私钥得保存好。

也就是说，那个id_rsa文件你得保存好，可以弄到U盘上，随身带着。而id_rsa.pub得改成系统默认识别的**authorized_keys**并保存在.ssh文件夹下

[(33条消息) ssh的用法，关于公钥和私钥_Become hunger become strong-CSDN博客_ssh私钥](https://blog.csdn.net/qq_34649947/article/details/80140465)

![image-20211206083832855](C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20211206083832855.png)

### 配置ssh



// 先卸载
sudo apt-get remove openssh-server
// 安装
sudo apt-get install openssh-server

//重启sshd服务
sudo service ssh --full-restart

1604是这样

![image-20211205123320398](C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20211205123320398.png)//自动启动
sudo systemctl enable ssh

![image-20211205130102939](C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20211205130102939.png)

##### ssh测试

最快的方法

在vmware中右键虚拟机-》SSH-》 CONECT TO SSH 具体可看上面

#### /etc/ssh/ssh_host_key

![image-20211205130552962](C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20211205130552962.png)

# sshconfig文件的含义

### Config

### bug1

![image-20211206084734588](C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20211206084734588.png)

## VMware

1虚拟机之间相互ping通，把他们放到同一个网里面

2VMtool

安装教程16.04d 记得先关机

[\安装VMware Tools选项显示灰色的正确解决办法 - 简书 (jianshu.com)](https://www.jianshu.com/p/df5537b8616a)



## 计网实验三

图3为在TCP客户端和TCP服务器端应用程序建立好TCP连接之前，在另一Shell窗口中，**使用**

```bash
ifconfig 确定其网卡
```



```bash
sudo tcpdump -i ens33 tcp port 6666 -w "tcpdump.log"
```

在TCP客户端与TCP服务器端应用程序通信结束后，在图3所示窗口中，用“Ctrl+C”终止此tcpdump命令的执行。Tcpdump命令退出，并将抓取的报文写入文件tcpdump.log中。



图4为使用“”命令显示tcpdump.log文件中存储的消息。

sudo tcpdump -i lo tcp port 6666 -w "tcpdump.log"

```bash
sudo tcpdump -r tcpdump.log
```

插入控制机制

重发

定时器（例子里面）

写到报告里面

send协议并不会发送10次tcp报文，因为他是把数据交给tcp协议，发送的次数是TCP的流量限制所决定的，这里的send是比较底层的，不是高级语言封装的，

接受一次打印的一般是几倍

![1_3双窗口客户端发送abc](D:\windowsFileFromC\桌面\a计网实验2\实验三\1_3双窗口客户端发送abc.png)

用其他语言也可以

![1_4双窗口tcpdum查看信息，可见笔记](D:\windowsFileFromC\桌面\a计网实验2\实验三\1_4双窗口tcpdum查看信息，可见笔记.png)

图5为用wireshark抓包软件打开图3中形成的tcpdump.log抓包文件。在Wireshark窗口中，可以看到抓取的TCP客户端和TCP服务器端之间传递的TCP消息。对应于图1和图2所示的这次通信过程，TCP客户端在与TCP服务器端建立了TCP连接后，客户端TCP协议向服务器端TCP协议发送了9条携带数据的TCP报文（消息编号：4、6、8、10、12），编号为20的TCP报文的FIN比特位为1，也是一条关闭TCP连接的TCP报文（参见图6）。



注意这里和老师的不一样，老师的初始长度为33 我的初始长度为0





![image-20211215105450236](C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20211215105450236.png)

![image-20211215115947158](C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20211215115947158.png)







模拟丢包

```bash
sudo iptables -A INPUT -s 127.0.0.1 -j DROP
```

![image-20211215112133740](C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20211215112133740.png)

```
sudo iptables -D INPUT -s 127.0.0.1 -j DROP
```



老师的图片

![image-20211215112820720](C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20211215112820720.png)

![image-20211215112648658](C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20211215112648658.png)

图11为用wireshark抓包软件打开图10中形成的tcpdump2.log抓包文件。图11中，编号为1、2、15的数据包是TCP连接的三次握手数据包。编号为16的数据包为客户端TCP协议发出的第一个数据包，TCP报文中的数据长度为4字节。编号为18的数据包为客户端TCP协议发出的第二个数据包，TCP报文中携带的数据长度为36个字节。编号为3、4、56、7、8、9、10的包为客户端TCP协议重传的数据包，注意这些重传的****TCP****报文间的时间间隔。



### IPtable

![image-20211215160445668](C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20211215160445668.png)

![image-20211215160537792](C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20211215160537792.png)

程序内使用

![image-20211215160250700](C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20211215160250700.png)



![image-20211215160631210](C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20211215160631210.png)随机函数

可以windows

停等协议，模拟丢包



428a2f98 71374491 b5c0fbcf e9b5dba5 3956c25b 59f111f1 923f82a4 ab1c5ed5 d807aa98 12835b01 243185be 550c7dc3 72be5d74 80deb1fe 9bdc06a7 c19bf174 e49b69c1 efbe4786 0fc19dc6 240ca1cc 2de92c6f 4a7484aa 5cb0a9dc 76f988da 983e5152 a831c66d b00327c8 bf597fc7 c6e00bf3 d5a79147 06ca6351 14292967

27b70a85 2e1b2138 4d2c6dfc 53380d13 650a7354 766a0abb 81c2c92e 92722c85 a2bfe8a1 a81a664b c24b8b70 c76c51a3 d192e819 d6990624 f40e3585 106aa070 19a4c116 1e376c08 2748774c 34b0bcb5 391c0cb3 4ed8aa4a 5b9cca4f 682e6ff3 748f82ee 78a5636f 84c87814 8cc70208 90befffa a4506ceb bef9a3f7 c67178f2

### Xshell XFTP协同编程

### visual studio文件编码问题

在“文件”中添加高级保存选项

![image-20211216110730661](C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20211216110730661.png)

如果没有高级保存选项

![image-20211216110856649](C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20211216110856649.png)

用下面这个添加

[VS进行编码格式的修改 - 青丝·旅人 - 博客园 (cnblogs.com)](https://www.cnblogs.com/Kirito-Asuna-Yoyi/p/VS-CodeFormatSetup.html#Two)

### 使用UDP设计可靠的协议

https://zhuanlan.zhihu.com/p/129218784

![image-20211216130105369](C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20211216130105369.png)

![image-20211216130149334](C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20211216130149334.png)

![image-20211216130210466](C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20211216130210466.png)





[(35条消息) 基于UDP的滑动窗口协议的设计与实现_udp滑动窗口-C++文档类资源-CSDN文库](https://download.csdn.net/download/hui_209/2788608?spm=1035.2023.3001.6557&utm_medium=distribute.pc_relevant_bbs_down.none-task-download-2~default~OPENSEARCH~default-1.nonecase&depth_1-utm_source=distribute.pc_relevant_bbs_down.none-task-download-2~default~OPENSEARCH~default-1.nonecase)

可以用于学习的示例代码（goback to n）



服务器Server

```c++
/* server.c - go-back-n server implementation in C
 * by Elijah Jordan Montgomery <elijah.montgomery@uky.edu>
 * based on code by Kenneth Calvert
 *
 * This implements a go-back-n server that implements reliable data
 * transfer over UDP using the go-back-n ARQ with variable chunk size
 *
 * for debug purposes, a loss rate can also be specified
 * compile with "gcc -o server server.c"
 * tested on UKY CS Multilab
 */
#include <stdio.h>		/* for printf() and fprintf() */
#include <sys/socket.h>		/* for socket() and bind() */
#include <arpa/inet.h>		/* for sockaddr_in and inet_ntoa() */
#include <stdlib.h>		/* for atoi() and exit() */
#include <string.h>		/* for memset() */
#include <unistd.h>		/* for close() */
#include <errno.h>
#include <memory.h>
#include <signal.h>
#include<iostream>
#include<string>
 //#include "gbnpacket.cpp"		/* defines go-back-n packet structure */

//#define ECHOMAX 255		/* Longest string to echo */
using namespace std;
const int MAX_BUF_LEN = 8096;
const int ECHOMAX = 255;

//下面的为数据包的类型
const int NORMAL_ACK = 2;
const int GOOD_BYE = 4;
const int GOOD_BYE_ACK = 8;

struct mypacket
{
	int type;
	int seq_no;
	int length;
	char data[512];
};
void Error_Message(string errorMessage);	/* External error handling function */
void Catch_Alarm(int ignored);
void Error_Message(string errorMessage)//打印错误消息
{
	printf("%s", errorMessage.c_str());//
	perror(errorMessage.c_str());
	exit(1);
}

void Catch_Alarm(int ignored) //与alarm函数绑定
{
	printf("CatchAlarm! Code(%d)\n", ignored);
	exit(0);
}

main(int argc, char* argv[])
{
	char buffer[MAX_BUF_LEN];		/* buffer with room for null byte */
	buffer[MAX_BUF_LEN-1] = '\0';		/* null terminate the buffer */
	int sock;			/* Socket */
	struct sockaddr_in serverAddr;	/* Local address */
	struct sockaddr_in clientAddr;	/* Client address */
	unsigned int clientAddrLen;	//客户端地址* Length of incoming message */
	unsigned short serverPort;	//本机接口* Server port */
	int recvMsgSize;		//收到信息的大小* Size of received message */
	int packet_rcvd = -1;		//上一次成功接收到的信息* highest packet successfully received */
	struct sigaction myAction; 
	double lossRate;		/* loss rate as a decimal, 50% = input .50 */


	bzero(buffer, MAX_BUF_LEN-1);		/* zero out the buffer */

	if (argc < 3 || argc > 4)		/* Test for correct number of parameters */
	{
		fprintf(stderr, "Usage:  %s <UDP SERVER PORT> <CHUNK SIZE> [<LOSS RATE>]\n", argv[0]);
		exit(1);
	}

	serverPort = atoi(argv[1]);	/* First arg:  local port */
	int chunkSize = atoi(argv[2]);	/* num bytes per chunk */
	if (argc == 4)
		lossRate = atof(argv[3]);	/* loss rate as percentage i.e. 50% = .50 */
	else
		lossRate = 0.0;			/*default to 0% intentional loss rate */

	//设置随机种子
	//srand48(123456789);/* seed the pseudorandom number generator */
	/* Create socket for sending/receiving datagrams */
	//注意，这里的Socket可以用于收/发
	if ((sock = socket(PF_INET, SOCK_DGRAM, IPPROTO_UDP)) < 0)//创建socket
		Error_Message("socket() failed");

	/* Construct local address structure */
	memset(&serverAddr, 0, sizeof(serverAddr));	/* Zero out structure */
	serverAddr.sin_family = AF_INET;	/* Internet address family */
	serverAddr.sin_addr.s_addr = htonl(INADDR_ANY);	/* Any incoming interface */
	serverAddr.sin_port = htons(serverPort);	/* Local port */

	/* Bind to the local address */
	//绑定
	if (bind(sock, (struct sockaddr*)&serverAddr, sizeof(serverAddr)) < 0)
		Error_Message("bind() failed");
	myAction.sa_handler = Catch_Alarm;
	//设置网络超时检测的方式
	if (sigfillset(&myAction.sa_mask) < 0)/*setup everything for the timer - only used for goodbye */
		Error_Message("sigfillset failed");
	myAction.sa_flags = 0;
	if (sigaction(SIGALRM, &myAction, 0) < 0)//安装SIGALRM信号,用于配合Alarm
		Error_Message("sigaction failed for SIGALRM");
	for (;;)			/* Run forever */
	{
		/* set the size of the in-out parameter */
		clientAddrLen = sizeof(clientAddr);
		struct mypacket currPacket; /* current packet that we're working with */
		memset(&currPacket, 0, sizeof(currPacket));//把这个字符设置为0
		/* Block until receive message from a client */
		recvMsgSize = recvfrom(sock, &currPacket, sizeof(currPacket), 0, (struct sockaddr*)&clientAddr, &clientAddrLen);//主要的接受函数 receive GBN packet */
		//ntohl将一个无符号长整形数从网络字节顺序转换为主机字节顺序，下面三个语句的含义为将接收到的字节流转为可识别的类型
		currPacket.type = ntohl(currPacket.type);
		currPacket.length = ntohl(currPacket.length); /* convert from network to host byte order */
		currPacket.seq_no = ntohl(currPacket.seq_no);
		if (currPacket.type == GOOD_BYE) // 关闭类型 4tear-down message */
		{
			printf("%s\n", buffer);
			struct mypacket ackmsg;
			ackmsg.type = htonl(GOOD_BYE_ACK);//确认类型8
			ackmsg.seq_no = htonl(0);//确认序号/*convert to network endianness */
			ackmsg.length = htonl(0);
			if (sendto(sock, &ackmsg, sizeof(ackmsg), 0,(struct sockaddr*)&clientAddr,clientAddrLen) != sizeof(ackmsg))
			{
				Error_Message("error sending goodbye ack"); /* not a big deal-data already rcvd */
			}
			//alarm函数的含义为，每隔7s给线程传递一个信息
			alarm(7);//重发的时间间隔为7s
			while (1)
			{
				while ((recvfrom(sock, &currPacket, sizeof(int) * 3 + chunkSize, 0,(struct sockaddr*)&clientAddr,&clientAddrLen)) < 0)
				{//收到回复包                                这里的3是因为有三个字节
					if (errno == EINTR)	//有警报 Alarm went off  */
					{
						/* never reached */
						exit(0);//结束进程
					}
				}
				if (ntohl(currPacket.type) == GOOD_BYE) //结束请求* respond to more goodbye messages */
				{
					ackmsg.type = htonl(GOOD_BYE_ACK);//8
					ackmsg.seq_no = htonl(0);//序号* convert to network endianness */
					ackmsg.length = htonl(0);//长度
					if (sendto(sock, &ackmsg, sizeof(ackmsg), 0, (struct sockaddr*)&clientAddr,clientAddrLen) != sizeof(ackmsg))//发送结束包的ACK/* send goodbye ack */
					{
						Error_Message("Error sending goodbye ack");
					}
				}
			}
			Error_Message("recvfrom() failed");
		}
		else
		{
			if (lossRate > drand48())//随机丢包率
				continue; /* drop packet - for testing/debug purposes */
			printf("received packet %d length %d\n", currPacket.seq_no, currPacket.length);

			/* Send ack and store in buffer */
			if (currPacket.seq_no == packet_rcvd + 1)
			{
				packet_rcvd++;
				int buff_offset = chunkSize * currPacket.seq_no;
				memcpy(&buffer[buff_offset], currPacket.data, /* copy packet data to buffer */
					currPacket.length);
			}
			printf("send ack no %d\n", packet_rcvd);
			struct mypacket currAck; /* ack packet */
			currAck.type = htonl(NORMAL_ACK); /*convert to network byte order */
			currAck.seq_no = htonl(packet_rcvd);
			currAck.length = htonl(0);
			if (sendto(sock, &currAck, sizeof(currAck), 0, (struct sockaddr*)&clientAddr,clientAddrLen) != sizeof(currAck))/* send ack */
				Error_Message("sendto() sent a different number of bytes than expected");
		}
	}
	/* NOT REACHED */
}

```



客户端client，

```c++
/* client.c - go-back-n client implementation in C
 * by Elijah Jordan Montgomery <elijah.montgomery@uky.edu>
 * based on code by Kenneth Calvert
 *
 * This implements a go-back-n client that implements reliable data
 * transfer over UDP using the go-back-n ARQ with variable chunk size
 *
 * for debug purposes, a loss rate can also be specified in the accompanying
 * server program
 * compile with "gcc -o client client.c"
 * tested on UKY CS Multilab
 */

#include <stdio.h>		/* for printf() and fprintf() */
#include <sys/socket.h>		/* for socket(), connect(), sendto(), and recvfrom() */
#include <arpa/inet.h>		/* for sockaddr_in and inet_addr() */
#include <stdlib.h>		/* for atoi() and exit() */
#include <string.h>		/* for memset() */
#include <unistd.h>		/* for close() and alarm() */
#include <errno.h>		/* for errno and EINTR */
#include <signal.h>		/* for sigaction() */
#include<iostream>
#include<string>
//2019211955



using namespace std;
const int TIME_OUT_VAL = 3;	/*重传所花时间*/
const int MAX_TRIES=3;	//最大尝试次数

//下面的为数据包的类型
const int NORMAL_PACKET = 1;
const int NORMAL_ACK = 2;
const int GOOD_BYE = 4;
const int GOOD_BYE_ACK = 8;


struct my_packet
{
	int type;//32位类型
	int seq_no;//32位，序列号
	int length;//32位，长度
	char data[512];//数据，最大为512字节
};

int tries = 0;		//记录尝试的次数	/* Count of times sent - GLOBAL for signal-handler access */
int base = 0;        //字节定位
int windowSize = 0;   //窗户大小
int sendflag = 1;     //如果》0为则发送

void Error_Message(string errorMessage);	/* Error handling function */
void Catch_Alarm(int ignored);	/* Handler for SIGALRM */
void Catch_Alarm(int ignored)	//alarm绑定
{
	tries += 1;
	sendflag = 1;
}

void Error_Message(string errorMessage)//打印错误消息
{
	perror(errorMessage.c_str());
	exit(1);
}

int max(int a, int b) {
	return a > b ? a : b;
}		/* macros that most compilers include - used for calculating a few things */
int min(int a, int b) {
	return a < b ? a : b;
}		/* I think gcc includes them but this is to be safe */

int main(int argc, char* argv[])
{   //具体可见server注释
	int sock;			/* Socket descriptor */
	struct sockaddr_in serverAddr;	/* Echo server address */
	struct sockaddr_in clientAddr;	/* Source address of echo */
	unsigned short serverPort;	/* Echo server port */
	unsigned int clinetAddrLen;	/* In-out of address size for recvfrom() */
	struct sigaction myAction;	/* For setting signal handler */
	char* serverIP;			/* IP address of server */
	int respLen;			/* Size of received datagram */
	int packet_received = -1;	/* highest ack received */
	int packet_sent = -1;		/* highest packet sent */
	char buffer[1024] = "abcdefghijklnm abcdefghijklmm1234567890";	/* buffer - randomly generated by me */
	const int datasize = 1024;	/* data buffer size */
	int chunkSize;		/* chunk size in bytes */
	int nPackets = 0;		/* number of packets to send */

	if (argc != 5)		/* Test for correct number of arguments */
	{
		fprintf(stderr,
			"Usage: %s <Server IP> <Server Port No> <Chunk size> <Window Size>\n",
			argv[0]);
		exit(1);
	}

	serverIP = argv[1];		/* First arg:  server IP address (dotted quad) */
	chunkSize = atoi(argv[3]);	/* Third arg: string to echo */
	serverPort = atoi(argv[2]);	/* Use given port */
	windowSize = atoi(argv[4]);
	if (chunkSize >= 512)
	{
		fprintf(stderr, "chunk size must be less than 512\n");
		exit(1);
	}

	nPackets = datasize / chunkSize;//1024/64
	if (datasize % chunkSize)//如果不能整除，则还需要一个包来传输
		nPackets++;			/* if it doesn't divide cleanly, need one more odd-sized packet */
	  /* Create a best-effort datagram socket using UDP */
	if ((sock = socket(PF_INET, SOCK_DGRAM, IPPROTO_UDP)) < 0)
		Error_Message("socket() failed");
	printf("created socket");

	/* Set signal handler for alarm signal */
	//设置网络超时检测的方式，绑定Catch_Alarm 函数 
	myAction.sa_handler = Catch_Alarm;
	if (sigfillset(&myAction.sa_mask) < 0)	/* block everything in handler */
		Error_Message("sigfillset() failed");
	myAction.sa_flags = 0;

	if (sigaction(SIGALRM, &myAction, 0) < 0)
		Error_Message("sigaction() failed for SIGALRM");
	// 建立套接
	/* Construct the server address structure */
	memset(&serverAddr, 0, sizeof(serverAddr));	/* Zero out structure */
	serverAddr.sin_family = AF_INET;
	serverAddr.sin_addr.s_addr = inet_addr(serverIP);	/* Server IP address */
	serverAddr.sin_port = htons(serverPort);	/* Server port */

	/* Send the string to the server */
	//nPacket 目标发送包个数
	//packet_received 收到ack包的个数（成功发送的包）
	while ((packet_received < nPackets - 1) && (tries < MAX_TRIES))
	{
		// printf ("in the send loop base %d packet_sent %d packet_received %d\n",
	   //      base, packet_sent, packet_received);
		if (sendflag == 1)
		{
			sendflag = 0;
			int win_idx; /*window size counter */
			for (win_idx = 0; win_idx < windowSize; win_idx++)
			{
				packet_sent = min(max(base + win_idx, packet_sent), nPackets-1 ); /* calc highest packet sent */
				struct my_packet currpacket; /* current packet we're working with */
				if ((base + win_idx) < nPackets)
				{
					memset(&currpacket, 0, sizeof(currpacket));
					printf("sending packet %d packet_sent %d packet_received %d windows_position %d\n",base + win_idx, packet_sent, packet_received,win_idx);

					currpacket.type = htonl(1); //转换为1/*convert to network endianness */ %d
					currpacket.seq_no = htonl(base + win_idx);//转换为序号
					int currlength;
					if ((datasize - ((base + win_idx) * chunkSize)) >= chunkSize) /* length chunksize except last packet */
						currlength = chunkSize;
					else
						currlength = datasize % chunkSize;
					currpacket.length = htonl(currlength);
					memcpy(currpacket.data, buffer + ((base + win_idx) * chunkSize), currlength);/*copy buffer data into packet */
					//发包 send packet 
					if (sendto(sock, &currpacket, (sizeof(int) * 3) + currlength, 0,(struct sockaddr*)&serverAddr, sizeof(serverAddr)) != ((sizeof(int) * 3) + currlength))
						Error_Message("sendto() sent a different number of bytes than expected");
				}
			}

		}
		/* Get a response */
		clinetAddrLen = sizeof(clientAddr);
		alarm(TIME_OUT_VAL);	//alarm是C/c++中定时提醒的函数 Set the timeout 
		struct my_packet currAck;
		while ((respLen = (recvfrom(sock, &currAck, sizeof(int) * 3, 0,(struct sockaddr*)&clientAddr,&clinetAddrLen))) < 0)
			if (errno == EINTR)//如果是超时 alarm返回一个错误	/* Alarm went off  */
			{
				if (tries < MAX_TRIES)	//尝试次数/* incremented by signal handler */
				{
					printf("timed out, %d more tries...\n", MAX_TRIES - tries);
					break;
				}
				else
					Error_Message("no response after many tries ,please check you network and server");//不能用%d哈哈哈
			}
			else
				Error_Message("recvfrom() failed");
			//如果没有回复，则跳过
			if (!respLen) {
				continue;
			}
			/* recvfrom() got something --  cancel the timeout */
			//收到数据	
			int acktype = ntohl(currAck.type);//主机顺序 /* convert to host byte order */
			int ackno = ntohl(currAck.seq_no);
			if (ackno > packet_received && acktype == NORMAL_ACK)//acktype
			{
				printf("received new ack no %d packet_received %d\n",ackno,packet_received); /* receive/handle ack */
				packet_received++;
				base = packet_received+1; /* handle new ack */
				if (packet_received == packet_sent) //所有的东西都收到了/* all sent packets acked */
				{
					alarm(0); /* clear alarm */
					tries = 0;
					sendflag = 1;
				}
				else /* not all sent packets acked *///如果不是所有的包都收到了Acked
				{
					tries = 0; /* reset retry counter */
					sendflag = 0;                   
					alarm(TIME_OUT_VAL); /* reset alarm */
				}
			}
			else
			{
				if(acktype==NORMAL_ACK)
					printf("drop un-inorder ack packet %d package_received %d", ackno, packet_received); //丢弃掉迟到或者错误的ACK
				else {
					printf("no respond ! check network ot server\n"); //压根没收到ACK
				}
			}
		
	}
	int ctr;
	struct my_packet goodbye;
	goodbye.type = htonl(GOOD_BYE);
	goodbye.seq_no = htonl(0);
	goodbye.length = htonl(0);
	sendto(sock, &goodbye, (sizeof(int) * 3), 0,
		(struct sockaddr*)&serverAddr, sizeof(serverAddr));
	close(sock); /* close socket */
	exit(0);
}



```

### 如何获得函数的名字



%s argv[0]





## 人工智能导论

第一次排名算法结果

autoglun

![image-20211220170347375](C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20211220170347375.png)

```python
#筛选数据集
AgePre=[['Age','Parch','Pclass','SibSp','Title','Fare','Embarked']]
字符类型
#进行one-hot编码
AgePre=pd.get_dummies(AgePre)
ParAge=pd.get_dummies(AgePre['Parch'],prefix='Parch')
SibAge=pd.get_dummies(AgePre['SibSp'],prefix='SibSp')
PclAge=pd.get_dummies(AgePre['Pclass'],prefix='Pclass')
#查看变量间相关性
AgeCorrDf=pd.DataFrame()
AgeCorrDf=AgePre.corr()
AgeCorrDf['Age'].sort_values()
```

```
#拆分实验数据与预测数据
experData=fullSel[fullSel['Survived'].notnull()]
preData=fullSel[fullSel['Survived'].isnull()]

experData_X=experData.drop('Survived',axis=1)
experData_y=experData['Survived']
preData_X=preData.drop('Survived',axis=1)

#导入机器学习算法库
from sklearn.ensemble import RandomForestClassifier,GradientBoostingClassifier,ExtraTreesClassifier
from sklearn.discriminant_analysis import LinearDiscriminantAnalysis
from sklearn.linear_model import LogisticRegression
from sklearn.neighbors import KNeighborsClassifier
from sklearn.tree import DecisionTreeClassifier
from sklearn.svm import SVC
from sklearn.model_selection import GridSearchCV,cross_val_score,StratifiedKFold

#设置kfold，交叉采样法拆分数据集
kfold=StratifiedKFold(n_splits=10)

#汇总不同模型算法
classifiers=[]
classifiers.append(SVC())
classifiers.append(DecisionTreeClassifier())
classifiers.append(RandomForestClassifier())
classifiers.append(ExtraTreesClassifier())
classifiers.append(GradientBoostingClassifier())
classifiers.append(KNeighborsClassifier())
classifiers.append(LogisticRegression())
classifiers.append(LinearDiscriminantAnalysis())
```





### github

写论文

https://github.com/Keldos-Li/typora-latex-theme#%E4%B8%8B%E8%BD%BD%E4%B8%8E%E5%AE%89%E8%A3%85

北邮实验报告模板

[lihao2333/TP_BUPT: 北京邮电大学实验报告模板(带封面的,非官方) (github.com)](https://github.com/lihao2333/TP_BUPT)

大三下考试题

[ipid/BuptSse-2016-AllExam: 北邮软件工程专业 2016 级必修课的考试真题（来自考试后回忆） (github.com)](https://github.com/ipid/BuptSse-2016-AllExam#软件项目管理spm期中)

数据链路层



[TKONIY/sliding-window-protocols: 北京邮电大学计网实验，模拟数据链路层的滑动窗口协议。 (github.com)](https://github.com/TKONIY/sliding-window-protocols)

情报汇总

[xianfei/BUPT-Course-Assistant: 北邮课程小助手——电脑端跨平台的课表、查成绩、看校内新闻平台，自带北邮WebVPN可校外使用 (github.com)](https://github.com/xianfei/BUPT-Course-Assistant)



北邮论文

[lw/doc at master · 4387163/lw (github.com)](https://github.com/4387163/lw/tree/master/doc)

[DaxNing/BUPT2021: 考研资料,2021年上岸北邮，考研过程中留下来的资料 (github.com)](https://github.com/DaxNing/BUPT2021)

论坛爬虫

[zcybupt/byr_bbs: 北邮人论坛爬虫 (github.com)](https://github.com/zcybupt/byr_bbs)

给比别人的

[ingbyr/bbs-byr-cn-kyzk: 北邮人论坛考研专刊系列 (github.com)](https://github.com/ingbyr/bbs-byr-cn-kyzk)

北邮人

[TingliangZhang/Torrent: 北邮人、北洋园、RuTracker的种子及下载设置 (github.com)](https://github.com/TingliangZhang/Torrent)

北邮机器学习大作业



[PouringRain/MachineLearningCourse: 北邮机器学习课程作业 (github.com)](https://github.com/PouringRain/MachineLearningCourse)

北邮人论坛

[WhymustIhaveaname/ByrBtAutoDownloader: 升级版的北邮人 BT 全自动下载刷流脚本。最近邀请有点多，可以留言找我要。 (github.com)](https://github.com/WhymustIhaveaname/ByrBtAutoDownloader)

北邮本科毕设

[phydx0803/BUPTReportTemplate: 一款基于北邮本科毕设标准的实验报告模板 (github.com)](https://github.com/phydx0803/BUPTReportTemplate)

知识图谱

[Shen-GuoXin/2019-QASystemofBUPTBasedOnKnowledgeMap: 2019-基于知识图谱的北邮校园信息化领域智能问答系统 (github.com)](https://github.com/Shen-GuoXin/2019-QASystemofBUPTBasedOnKnowledgeMap)



情报汇总

[SimonGH0STRiley/AirConditioningManagementSystem](https://github.com/SimonGH0STRiley/AirConditioningManagementSystem)

[chyroc/byr-topten: 北邮人论坛十大热帖历史合集 (github.com)](https://github.com/chyroc/byr-topten)

https://github.com/liangxun/DataMining

[byrwiki/byrwiki: 北邮人导航：一个框，全能搜 (github.com)](https://github.com/byrwiki/byrwiki)

打卡

[Qianmoxsn/BUPT_dailycheck-: 运行于本地的北邮每日晨午晚检填报 (github.com)](https://github.com/Qianmoxsn/BUPT_dailycheck-)

### 陶瓷

![image-20220331162821190](C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20220331162821190.png)

李老师您好，我想问一下您的实验室往年专硕名额是多少呢？如果名额足够的话，我能在4月中旬前往您实验室做一些辅助性工作吗？（目前在校）

 我是来自计算机学院软件工程专业的2019级本科生陈可淇，上学期选过您的人工智能导论课，也听沛霖和子睿描述过您实验室的情况，所以前来咨询一下您实验室的情况。

下面简单介绍一下我的情况。

科研情况：

我目前正参与两个人工智能领域的科研工作：

·  一篇是nlp方向的命名实体识别任务，我主要负责模型实现，目前谈好的是共一，但是目前的实验遇到了较大瓶颈，论文投刊时间未知。

·  另一篇是关于轨迹预测方向，我主要负责数据爬取和清洗、论文写作和模型调参，我大概能拿到二作或者三作，目前实验进展顺利，论文预计4月中旬投出。

其他情况：

· 但是我目前阅读和复现的论文大多数为命名实体识别和轨迹预测方向，对语音识别和情感计算方向了解不算多，

· 目前的智育排名为13.9%（院保研大约20%）这样，能够拿到保研名额，但是排名不算高。

· 除了论文和实验经历外，我也有一定的算法竞赛经历，英语水平为雅思6.0，同时工程能力尚可，有训练常见NLP模型的经验。

**·**





此外，我目前在校，您可以随时面试我。我也希望能够在4月中旬前往您实验室做一些辅助工作。（我的论文工作预计4月中旬完成）

特以图片方式附上我的简历，您也可以从附件下载。

谢谢您，期待您的回复。





"颉夏青"<xiexiaqing@bupt.edu.cn>;

 我是来自计算机学院软件工程专业的2019级本科生陈可淇，从同院同学处得到你的邮箱，冒昧打扰了。

   我一直对NLP方向保持关注与兴趣，并且今年暑假留校，有充分的时间学习和科研。

我本科的专业是软件工程，一直保持专业前10%的成绩 (GPA:3.74/4.0 排名：13/168)，也有过一些项目经历（附简历），自认为是一个踏实学习、力求上进的学生，希望有一个机会展示给您。

虽然我当前对NLP方向的了解还不够深不够多，但我计划在暑假时间里对NLP方向进行学习和研究，也很希望您能给我一个机会，加入您指导的本科研究组。

特以图片方式附上我的简历，您也可以从附件下载。

谢谢您，期待您的回复。

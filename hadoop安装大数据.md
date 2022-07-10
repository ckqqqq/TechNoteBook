# 实验一 hadoop安装

http://dblab.xmu.edu.cn/blog/install-hadoop/

http://dblab.xmu.edu.cn/blog/install-hadoop-cluster/

https://www.cnblogs.com/qinqiao/p/pseudo-distributed-hdfs-wordcount.html

https://blog.csdn.net/weixin_41374755/article/details/107146445

清华镜像

https://mirrors.tuna.tsinghua.edu.cn/apache/hadoop/common/stable/



## 实验目的

安装单机伪分布式Hadoop并运行程序，熟悉hadoop集群的部署操作。

实验内容

1. 每人在自己本地电脑上正确安装和运行伪分布式Hadoop系统。

2. 安装完成后,自己寻找一组英文网页数据,在本机上 运行Hadoop系统自带的WordCount可执行程序文件 ,并产生输出结果 

3.  实验结果提交：要求书写一个实验报告，其中包括：

   * 系统安装运行的情况 

   *  实验数据说明（下载的什么网页数据，多少个HTML或text文件)  
   *  程序运行后在Hadoop Web作业状态，查看界面上的作业运行状态屏幕拷贝 
   *  实验输出结果开头部分的屏幕拷贝 
   *  实验体会

## 实验环境

## 硬件环境

x86笔记本电脑，Intel Core i5，NVIDIA GeForce MX150，50GB RAM

## 网络环境

校园网WiFi环境

## 软件环境

**hdoop版本2.10.1**

**jdk版本1.8**

阿里云服务器Ubuntu20.04 server ESC服务器

Ubuntu20.04 Desktop 虚拟机

VMware

XShell XFTP Xmanager等远程ssh工具

## 实验结果

一共尝试以下实验

  实验名称            实验平台           结果   遇到的困难和解决方法
------------------- ------------------ ------ ----------------------
  部署并运行haoop伪分布式配置 阿里云ESC服务器   成功   见附录
  部署并运行haoop伪分布式配置    虚拟机             成功   见附录

## 实验方案

## 总体方案设计





## 实验结果

![image-20220403212254076](C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20220403212254076.png)

结果截图，过程见“实验过程”

## 系统安装运行的情况



## 实验数据说明

实验数据一

文件夹中所有.xml文件



实验数据二

## 程序运行后在HadoopWeb作业界面查看作业运行状态截图

程序运行后在8088端口，启用yarn后的web截图



查看其具体信息

![image-20220404124442482](C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20220404124442482.png)

![img](D:\社交软件\QQinfo\1047969038\Image\C2C\2{SK3E[%8R_[~3`SZTUUFBM.png)

![image-20220404234244840](C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20220404234244840.png)





![image-20220403215244521](C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20220403215244521.png)



## 实验输出结果开头部分的屏幕拷贝



### wordcount运行界面截图（开头部分）

![image-20220404232629721](C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20220404232629721.png)

### Wordcount运行界面（长截图）

![image-20220404232441056](C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20220404232441056.png)

### wordcount的结果（开头部分）

![image-20220404233632769](C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20220404233632769.png)

### wordcount的结果（长截图）

![image-20220404232411987](C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20220404232411987.png)



## 实验过程

## 环境准备：配置虚拟机\配置云服务器

可以选择在VMware中的虚拟机中安装，也可以选择阿里云服务器安装，两种安装方式笔者都尝试过，

但是值得注意以下几点：

* 由于hadoop消耗较多内存和CPU资源，,阿里云虚拟机请选择较多资源的虚拟机，笔者选择的ESC虚拟机（双核 2G-40G）运行hadoop时经常崩溃，建议选择内存较多CPU性能较强的云服务器

* 运行阿里云ESC虚拟机请在防火墙处请开放如下端口

* ![image-20220405191434409](C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20220405191434409.png)

  开放上述端口后，才可以通过本机浏览器远程访问hadoop webUI地址为

  http://阿里云IP:50070/

  http://阿里云IP:8088/

  http://阿里云IP:特定端口/

* 本实验针对Ubuntu虚拟机，如果用的是 CentOS/RedHat 系统，请查看相应的[CentOS安装Hadoop教程_单机伪分布式配置](http://dblab.xmu.edu.cn/blog/install-hadoop-in-centos/)

## 环境准备：配置ssh免密登录



集群、单节点模式都需要用到 SSH 登陆（类似于远程登陆，你可以登录某台 Linux 主机，并且在上面运行命令），Ubuntu 默认已安装了 SSH client，此外还需要安装 SSH server：

```bash
sudo apt-get install openssh-server
```

Shell 命令

安装后，可以使用如下命令登陆本机：

```bash
ssh localhost
```

Shell 命令，如果登陆时需要每次输入密码，我们需要配置成SSH无密码登陆比较方便，便于hapoop操作。

首先退出刚才的 ssh，就回到了我们原先的终端窗口，然后利用 ssh-keygen 生成密钥，并将密钥加入到授权中：

```bash
exit                           # 
ssh localhostssh-keygen -t rsa              # 都按回车
cd /root/.ssh
cat /root/.ssh/id_rsa.pub >> /root/.ssh/authorized_keys       # 加入授权
ssh localhost #如果不需要密码就算成功
```

ssh localhost免密登录成功界面

![image-20220325133444614](C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20220325133444614.png)



## 步骤一：安装java环境

### 下载jdk1.8安装包

https://mirrors.tuna.tsinghua.edu.cn/AdoptOpenJDK/8/jdk/arm/linux/

```bash
wget https://mirrors.tuna.tsinghua.edu.cn/AdoptOpenJDK/8/jdk/arm/linux/OpenJDK8U-jdk_arm_linux_hotspot_8u322b06.tar.gz
```

![image-20220325124049087](C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20220325124049087.png)

### 解压

```bash
tar -zxvf 安装包名
```

![image-20220325124102287](C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20220325124102287.png)

### 移动并重命名JDK包。

下载java1.8 可以选择ARM或者X64



```bash
wget XXX .tar.gz
tar -zxvf hadoop-2.10.1.tar.gz -C /java-se-8u41-ri/
mv java-se-8u41-ri/ /usr/java8
```

![image-20220325124140202](C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20220325124140202.png)

### 配置Java环境变量。

```bash
echo 'export JAVA_HOME=/usr/java8' >> /etc/profile
echo 'export PATH=$PATH:$JAVA_HOME/bin' >> /etc/profile
source /etc/profile
```

![image-20220325124201558](C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20220325124201558.png)

5.执行以下命令，查看Java是否成功安装。

```bash
java -version #注意不是java --version （离大谱了）
```

**此处碰到问题**

## 步骤二：下载hadoop

### 下载Hadoop安装包（2.10.1）

```bash
wget https://mirrors.tuna.tsinghua.edu.cn/apache/hadoop/common/hadoop-2.10.1/hadoop-2.10.1.tar.gz
```

![image-20220325125509168](C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20220325125509168.png)

### 解压Hadoop安装包

解压Hadoop安装包至/opt/hadoop （记住该地址）

https://mirrors.tuna.tsinghua.edu.cn/apache/hadoop/common/current2/

```bash
tar -zxvf hadoop-2.10.1.tar.gz -C /opt/
mv /opt/hadoop-2.10.1 /opt/hadoop
```

### 配置Hadoop环境变量。

```bash
echo 'export HADOOP_HOME=/opt/hadoop/' >> /etc/profile
echo 'export PATH=$PATH:$HADOOP_HOME/bin' >> /etc/profile
echo 'export PATH=$PATH:$HADOOP_HOME/sbin' >> /etc/profile
source /etc/profile    
```

![image-20220325130209802](C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20220325130209802.png)

### 添加Java路径

（如果已将java加入环境变量可以跳过这一步）

执行以下命令，修改配置文件yarn-env.sh和hadoop-env.sh。

```bash
echo "export JAVA_HOME=/usr/java8" >> /opt/hadoop/etc/hadoop/yarn-env.sh
echo "export JAVA_HOME=/usr/java8" >> /opt/hadoop/etc/hadoop/hadoop-env.sh
```

![image-20220325132726184](C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20220325132726184.png)

### 测试Hadoop是否安装成功。

```bash
hadoop version
```

如果返回以下信息，则表示安装成功。

![image-20220325132750229](C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20220325132750229.png)

### 各xml配置文件含义

一般来说配置文件夹路径为

```bash
所安装的路径/etc/hadoop/
```

下文中操作的所有xml文件皆是在该文件夹中的，下文主要有以下几个配置文件要修改：
hadoop-env.sh:Hadoop环境变量设置
core-site.Xml:主要完成NameNode的iP和端口设置
hdfs-site.Xml:主要完成HDFS的数据块副本等参数
设置
mapred-site.Xml:主要完成JobTracker IP和端口设置，能够设置yarn的WebUI
conf/slaves:完成Slaves节点IP设置
注：这个过程仅需在主节点上进行，然后将随着主机上安装
好的Hadoop目录一起复制到所有从节点

可以通过下列命令查看XML配置文件

```bash
cd  所安装的路径/etc/hadoop/
#本例中为 /opt/hadoop/etc/hadoop/
ls #可查看xml配置文件
```





## 步骤三：运行伪分布式hadoop

### .修改Hadoop配置文件core-site.xml。

- 执行以下命令开始进入编辑页面。

```bash
sudo apt-get install vim
vim /opt/hadoop/etc/hadoop/core-site.xml
```

- 节点内插入如下内容。
- 分别指定临时文件路径和core-site端口
- Core-site.xml

```XML
<configuration>
    <property>
        <name>hadoop.tmp.dir</name>
        <value>file:/usr/local/hadoop/tmp</value>
        <description>Abase for other temporary directories.</description>
    </property>
    <property>
        <name>fs.defaultFS</name>
        <value>hdfs://localhost:9000</value>
    </property>
</configuration>
```

- 按i进入编辑模式，按Esc键退出编辑模式，输入:wq保存退出。

  ![image-20220325133219759](C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20220325133219759.png)

  

  ### 修改Hadoop配置文件hdfs-site.xml

- 修改Hadoop配置文件hdfs-site.xml，执行以下命令开始进入编辑页面。

```bash
vim /opt/hadoop/etc/hadoop/hdfs-site.xml
```

- hdfs-site.xml

```xml
<configuration>
    <property>
        <name>dfs.replication</name>
        <value>1</value>
    </property>
    <property>
        <name>dfs.namenode.name.dir</name>
        <value>file:/usr/local/hadoop/tmp/dfs/name</value>
    </property>
    <property>
        <name>dfs.datanode.data.dir</name>
        <value>file:/usr/local/hadoop/tmp/dfs/data</value>
    </property>
</configuration>
```

- 常见端口介绍

| 端口  | 作用                                                         |
| :---- | :----------------------------------------------------------- |
| 9000  | fs.defaultFS，如：hdfs://172.25.40.171:9000                  |
| 9001  | dfs.namenode.rpc-address，DataNode会连接这个端口             |
| 50070 | dfs.namenode.http-address                                    |
| 50090 | dfs.namenode.secondary.http-address，如：172.25.39.166:50090 |
| 50020 | dfs.datanode.ipc.address                                     |
| 50475 | dfs.datanode.https.address                                   |
| 50010 | dfs.datanode.address，DataNode的数据传输端口                 |
| 8088  | yarn.resourcemanager.webapp.address，YARN的http端口          |

## 步骤四：启动Hadoop伪分布式

### 格式化HDFS文件系统

**警告：该命令不可重复执行，否则执行后可能导致出现start-yarn卡死问题**

```bash
hadoop namenode -format
```

![image-20220325141140357](C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20220325141140357.png)

### 启动Hadoop

遇到问题 上面的命令执行得特别慢，环境：阿里云

解决方法：重启阿里云系统，阿里云ESC服务器空间太小导致

碰到两个问题一是要输入密码



```bash
依次执行以下命令，启动Hadoop。
start-dfs.sh
```

![image-20220326194537142](C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20220326194537142.png)

正常运行截图如上

如果此处出现错误请看文末的错误与调试模块

### 查看已启动进程

启动成功后，执行以下命令，查看已成功启动的进程。

启动完成后，可以通过命令 `jps` 来判断是否成功启动，若成功启动则会列出如下进程:

* NameNode 
* DataNode
* SecondaryNameNode`
* jps

```
jps
```



![image-20220404123340592](C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20220404123340592.png)

问题：为什么启动 Hadoop 后，见不到书上所说的 JobTracker 和 TaskTracker。

答案：这是因为新版的  Hadoop 使用了新的 MapReduce 框架（ YARN，Yet Another Resource  Negotiator）。

问题：如果未出现上述进程怎么办？

答案：见后文错误与调试模块

### 浏览器访问（50070）

```http
https://阿里云公网IP:50070 #如果用阿里云服务器，请确保内存足够&防火墙开放
https://localhost:50070 #如果在 本机访问
```

显示如下界面则表示Hadoop伪分布式环境搭建完成。
![在这里插入图片描述](https://img-blog.csdnimg.cn/20200826151437237.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L2dhbmd5aWtlamk=,size_16,color_FFFFFF,t_70#pic_center)

## 步骤五：配置并且启动Yarn

这里是mapreduce的yarn配置

### 什么是yarn

YARN 是从 MapReduce 中分离出来的，负责资源管理与任务调度。YARN 运行于 MapReduce 之上，提供了高可用性、高扩展性，YARN 的更多介绍在此不展开，有兴趣的可查阅相关资料。

上述通过 `start-dfs.sh` 启动 Hadoop，仅仅是启动了 MapReduce 环境，我们可以启动 YARN ，让 YARN 来负责资源管理与任务调度。

### 修改mapred-site.xml

首先修改配置文件 **mapred-site.xml**，这边需要先进行重命名：

```bash
cd /opt/hadoop/etc/hadoop/
mv mapreduce.xml.template mapreduce.xml
vim mapreduce.xml
```

- mapreduce.xml
- 指定yarn为mapreduce的框架

```xml
<configuration>
    <property>
        <name>mapreduce.framework.name</name>
        <value>yarn</value>
    </property>
</configuration>
```

**修改yarn-site.xml**

进入配置文件夹

```bash
vim yarn-site.xml
```



```xml
<configuration>
    <property>
        <name>yarn.nodemanager.aux-services</name>
        <value>mapreduce_shuffle</value>
        </property>
</configuration>
```

### 启动yarn

```
start-yarn.sh      # 启动YARN
mr-jobhistory-daemon.sh start historyserver  # 开启历史服务器，才能在Web中查看任务运行情况
```

### 查看已成功启动的进程

上面是出现的错误一3.启动成功后，执行以下命令，查看已成功启动的进程。

```
jps
```

![image-20220326194654626](C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20220326194654626.png)

### 服务器访问（8088）

```http
https://阿里云公网IP:8088 #如果用阿里云服务器，请确保内存足够&防火墙开放
https://localhost:8088 #如果在 本机访问
```

![image-20220404124442482](C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20220404124442482.png)

成功界面如上（没有Wordcount任务）



### 停止hadoop运行

```bash
 stop-all.sh
```

或者

```
 stop-dfs.sh
 stop-yarn.sh
```

### 

## 步骤六：运行wordcount程序

问题：hadoop fs 和hdfs dfs区别

[(41条消息) hadoop fs、hadoop dfs与hdfs dfs命令的区别及hadoop fs命令说明_Shyllin的博客-CSDN博客_fs是什么意思](https://blog.csdn.net/Shyllin/article/details/88663017)

### #在hadoop中建立input文件夹

```bash
hdfs dfs -mkdir input 
```

### 将hadoop本地文件夹放入input文件夹中

```bash
hdfs dfs -ls input
```

### 查看input文件夹

```bash
hdfs dfs -put ./etc/hadoop/*.xml input #此时结果应该是一堆xml文件
```

![image-20220326203641933](C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20220326203641933.png)

### 寻找example文件

如果版本为hadoop2.X，则一般来说该路径下会存在 hadoop-mapreduce-examples-2.10.1.jar 文件，如下图

```bash
安装文件夹/share/hadoop/mapreduce
我的如下 /usr/local/hadoop/share/hadoop/mapreduce/hadoop-mapreduce-examples-2.10.1.jar
```

![image-20220405200345628](C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20220405200345628.png)

### 运行wordcount

命令为

```
hadoop jar /usr/local/hadoop/share/hadoop/mapreduce/hadoop-mapreduce-examples-2.10.1.jar wordcount input /xml_output/
```

解释

```bash
hadoop jar example所在路径/hadoop-mapreduce-examples-2.10.1.jar workcount  输入文件名 输出文件夹位置
```



![image-20220404232441056](C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20220404232441056.png)

### 查看wordcount的结果

web端可看运行状态

![image-20220404124442482](C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20220404124442482.png)

```
hdfs dfs -get xml_output ./xml_output 
#解释hdfs dfs -get HDFS上输出文件夹 ./本地文件夹
cat ./xml_output/* 
#查看结果
```

![image-20220404232411987](C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20220404232411987.png)

## 实验收获

## 问题与调试

本次大数据实验笔者遇到了无数是问题T_T，下面是笔者遇到的问题与解决方法，可供大家参考

## 问题一：启动伪分布式时缺少 datanode/namenode/secondary/

![image-20220403155931602](C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20220403155931602.png)

启动完成后，可以通过命令 `jps` 来判断是否成功启动，若成功启动则会列出如下进程:

* NameNode

  检查xml文件配置  

* DataNode 

  见后文 [datanode无法启动问题 - 夏末秋凉 - 博客园](http://8.142.92.175:8088/)

* SecondaryNameNode 

  ```
  stop-all.sh
  start-dfs.sh
  ```

  

![image-20220404123340592](C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20220404123340592.png)

## 问题二：报错如下

There are 0 datanode(s) running and no node(s) are excluded in this operation.、

解决方法：https://blog.csdn.net/weixin_41374755/article/details/107146445

## 问题三：启动yarn时卡死（这个卡了我半天）

```bash
start-yarn.sh
```

![image-20220326194619108](C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20220326194619108.png)

解决方法：

出现上述问题可能是格式化两次hadoop，导致没有datanode
解决方法1：重启linux,再使用start-dfs.sh和start-yarn.sh 重启一下hadoop
解决办法2：找到hadoop安装目录下 hadoop-2.4.1/data/dfs/data里面的current文件夹删除



## 问题四：启动dfs时出现以下错误

![image-20220325134233714](C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20220325134233714.png)

解决方法：hdfs-site.xml配置错误，检查配置

## 问题五：connect错误

![image-20220403211453780](C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20220403211453780.png)

解决方式：.

检查ssh

启动yarn

![image-20220403211536586](C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20220403211536586.png)



## 问题六：hdfs dfs -mkdir错误

解决方法：

![image-20220403210304944](C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20220403210304944.png)

## 问题七：Connect Refuse

bug

mkdir: Call From iZ8vbhsfhga8yj95cx1410Z/172.19.51.155 to localhost:9000 failed on connection exception: java.net.ConnectException: Connection refused; For more details see:  http://wiki.apache.org/hadoop/ConnectionRefused

![image-20220403160727744](C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20220403160727744.png)

解决方法：检查yarn配置，



## 问题八 ：服务器卡死

原因：阿里云内存和CPU资源不足，阿里云差评！

解决方法：

使用top命令kill掉占用大量资源的进程，重新启动阿里云服务器&服务器升级扩容，换服务器。

![image-20220403212457291](C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20220403212457291.png)

## 实验心得

本次实验过程将在4月10日前上传到我的CSDN 博客上(**用户名: ckqqqqq)**。连接还没有出来，因为博客图床还在审核中。

本次大数据实验中我大约碰到了10个问题，这些问题的原因和解决方法我总结如上（见问题与调试模块），在解决问题的过程中我加深了对linux和hadoop的理解，提升了我的实践能力。

此外除了**在阿里云上配置hadoop伪分布式外**，我还在自己的**虚拟机上尝试过配置hadoop伪分布式。**总的来说，后者比前者容易，因为前者要考虑防火墙和服务器资源等问题。

# 实验三：hbase安装

[“dlcdn.apache.org”A记录/cname检测结果--Dns查询|dns查询--站长工具 (chinaz.com)](https://tool.chinaz.com/dns?type=1&host=dlcdn.apache.org&ip=)、

![image-20220527004502574](C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20220527004502574.png)

```
suod vim /etc/hosts
151.101.2.132 dlcdn.apache.org
sudo /etc/init.d/networking restart
```

[HBase2.2.2安装和编程实践指南_厦大数据库实验室博客 (xmu.edu.cn)](http://dblab.xmu.edu.cn/blog/2442-2/)



```
curl -O https://mirrors.tuna.tsinghua.edu.cn/apache/hbase/2.4.12/hbase-2.4.12-bin.tar.gz
```

 

ps:linux上装idea的时候，记得要直接在bin下

```
source idea.sh
```


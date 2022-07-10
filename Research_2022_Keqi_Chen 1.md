---
typora-copy-images-to: upload
---

#  Research_2022

报告的主体部分为 “任务一：具有共情能力的对话生成-调研报告”

目录😼🍔🍔🍔

[TOC]



## 重要数据

### 重要的网址：论文报告/组会顺序/要读的论文

https://docs.qq.com/sheet/DSWhFVGZYRExzZGtZ?tab=BB08J2

### 重要的：周记/PPT/文档上传

10.112.243.253

[MM-Wiki - Login](http://10.112.243.253:8081/author/index)

每个人汇报后在这里说汇报了哪些文章ppt可以上传

每个人汇报后在这里说汇报了哪些文章ppt可以上传

论文笔记

https://readpaper.com/

![image-20220526133956742](https://s2.loli.net/2022/07/05/6h5vTSZ9JQUkKEG.png)

## 任务一：具有共情能力的对话生成-调研报告

**介绍**&**定义**

​    开放域对话系统在生成流畅和相关回复方面取得了成功。然而，人们在与机器交谈时，仍然可以感觉到人与机器之间存在明显的差距。其中一个主要原因是现有的对话系统缺乏情感理解和同理心。而我们的目标就是赋予对话系统情感理解和同理心回复的能力，

### 智源YSSNLP回放

https://event.baai.ac.cn/event/408

### 智源YSSNLP 会议 对话生成主题

**腾讯的研究员**

腾讯ailab的三大方向

文本理解 文本生成 机器翻译

今天的主题：开放域对话系统生成

预训练对话模型-（dialog-gpt fine tuning 

![image-20220629162000833](https://s2.loli.net/2022/07/05/x6TEwu5y3C2Jiq4.png)





### 智源YSSNLP 会议 情感计算主题

趋势方向：情绪识别

对话

情绪识别在细分的时候有区别。情绪识别在对话中应用更难，

随着两个人的对话可能会剧烈变化

历史更短

心理学结合

更难

情感计算

计算难度极大，受到诸多条件的限制

比如一个人打了你一巴掌

比如情侣/陌生人

高度个性化的机制

大规模的预训练模型提供了一个机制，但是情感是高度个性化的，进一步推理

不同的情感生成不同的回复

根据情感背后的原因:其实就是情和理，不仅仅是文本的，有可能是多模态的信息，

#### 对话生成国内主要的研究组：

哈工大 徐睿峰教授 

情感分析  情感原因发现 立场检测 论辩分析 他们也做情感文本生成

[Improving Empathetic Response Generation by Recognizing Emotion Cause in Conversations (aclanthology.org)](https://aclanthology.org/2021.findings-emnlp.70.pdf)

Improving Empathetic Response Generation by Recognizing Emotion Cause in Conversations（EMNLP2021）-识别对话中的情绪因素

武汉大学 NLPWM 课题组 

方 面词识别 方面情感分类  端到端情感分类



多模态情感分析任务中

多模态融合，大部分工作使用transformer将一种模态作为Query一种作为Key 和 value 

特征交互：残差连接

特征融合方式：拼接、非线性变化、线性变哈、任务特定融合方式

残差连接



![image-20220629154419354](https://s2.loli.net/2022/07/05/B51TxrEu2cbgOsI.png)



Zhuang Chen, Tieyun Qian: Enhancing Aspect Term Extraction with Soft Prototypes.EMNLP 2020-低资源下方面词抽取

![image-20220629153645909](https://s2.loli.net/2022/07/05/JsAuakFZTo9CDdq.png)

清华大学 COLAB 共情对话

[[2106.01144\] Towards Emotional Support Dialog Systems (arxiv.org)](https://arxiv.org/abs/2106.01144)

[[2105.08316\] CoMAE: A Multi-factor Hierarchical Framework for Empathetic Response Generation (arxiv.org)](https://arxiv.org/abs/2105.08316)

[[2106.01702\] PsyQA: A Chinese Dataset for Generating Long Counseling Text for Mental Health Support (arxiv.org)](https://arxiv.org/abs/2106.01702)

[[2109.05739\] CEM: Commonsense-aware Empathetic Response Generation (arxiv.org)](https://arxiv.org/abs/2109.05739)

![image-20220629151045882](https://s2.loli.net/2022/07/05/hNdoeY68cfIEvU3.png)



![image-20220629151215862](https://s2.loli.net/2022/07/05/P9HeYi1Mwl2XTbK.png)![image-20220629151218211](https://s2.loli.net/2022/07/05/P9HeYi1Mwl2XTbK.png)

清华

对话生成系统的综述

[对话生成预训练模型速览 - 知乎 (zhihu.com)](https://zhuanlan.zhihu.com/p/428382078)

对话生成的国外论文

[csnlp/Dialogue-Generation: A Paper List for Open-Domain Dialogue Generation, and related datasets. (github.com)](https://github.com/csnlp/Dialogue-Generation)

细粒度情感分析

### 历史

#### 较早期的工作：2018-

· MIT教授Posalind开创了情感计算的方向

· UIC的刘兵教授开创了文本领域的情感分析方向

· 比较具有开创性的一篇论文:ECM   将情感引入对话生成系统中

#### 近5年的工作

![image-20220622083753239](https://s2.loli.net/2022/07/05/IocBsPk9rjA7qdZ.png)

### 共情能力的对话生成的细分方向（综述）

或者说基础工作

**Emotion Understanding:**

机器是否可以理解情绪? 并通过文本等形式表征出来？

**Emotional Chatting:** （主要）

如果认为计算机可以理解情绪，那么人机对话时该如何表达情绪?

**Empathetic Dialog:** （主要）

在理解用户的情绪后，机器应该表达什么样的情绪?

**Emotional Support:**（主要）

多轮交互下，如何使得用户愿意持续和机器对话并最终缓解用户的情绪问题？

### 方向一：ECM介绍（2018）：生成具有特定情感的response

什么是生成具有特定情感的response？就是让机器生成happy/sad/angry的答复

**主要任务：生成特定方向的回复**

ECM全称为Emotion Chat Machine

**[ Emotional Chatting Machine: Emotional Conversation Generation with Internal and External Memory](https://link.zhihu.com/?target=https%3A//arxiv.org/abs/1704.01074)**



https://link.zhihu.com/?target=https%3A//github.com/tuxchow/ecm

**这篇论文是共情对话生成领域一篇比较具有开创性的论文（首次将情感因素引入了基于深度学习的生成式对话系统，定义和尝试探索共情对话生成问题）**

#### 模型结构



![image-20220622082413383](https://s2.loli.net/2022/07/05/il2ngd18L5WDsEO.png)

GRU（LSTM++）

#### 主要技术

**Emotion category embedding**

对**情感的高层次抽象，情感嵌入为向量**，将这个句子的情感类别作为Decoder输入的一部分，

![image-20220622091315303](https://s2.loli.net/2022/07/05/qjyFKsxkpUcf63O.png)

将query编码后变成向量

**Emotion internal state**

![image-20220622091620111](https://s2.loli.net/2022/07/05/Ts7caVfNq8JGbxA.png)

 $$内部记忆模型: 这个部分主要完成了两件事：当机器准备生成第 t 个应答词，有多大概率使用当前状态的情感状态M_{e,t}^{l}，并更新下一时刻t+1的情感状态。$$

用户在表达一句话时，是有一个潜在的情感状态的（开心、伤心等等）

比如将Sad表达成一个state，每经过一个gate他们的情感向量状态会衰减，最后出来的时候向量的情感状态变成0

认为当一句话表达完后，他的情感状态最后为0

$$S_1-{decode}>Y_1$$



![image-20220622085343184](https://s2.loli.net/2022/07/05/kmNqBysvLHl5ZJ2.png)

**Emotion external memory**

将具有强烈情感表达的词同比较generic的词分开对待，比如（Lovely）和（Person）

具体解决方案是会有一个字典，字典里面存了一个词的情感表达有多么强烈

![image-20220622085637821](https://s2.loli.net/2022/07/05/vatOex9pYcLdbMV.png)



#### 可用数据集

原有数据集：

| 名称            | 作者         | 解释                                                         | 下载 |
| --------------- | ------------ | ------------------------------------------------------------ | ---- |
| NLPCC 2013&2014 | NLPCC        | 对微博的一个情感分类2万句子                                  | F    |
| STC数据集       | Lifeng shang | 微博的一个对话数据，两万的对话数据每轮对话大概20多个response 用情感分类器标注 | T    |
|                 |              |                                                              | ?    |
|                 |              |                                                              |      |



#### 评价指标

自动评价。人工评价

对情感分类生成任务上的准确率，（嘿，机器，生成sad的数据）

![image-20220622090509317](https://s2.loli.net/2022/07/05/vEjuyL7wUJ2KQSX.png)

他们生成的回复，5分类

![image-20220622082348681](https://s2.loli.net/2022/07/05/KCgq3YSW8J5Blyw.png)

------------------------------------------------
人类的对话行为中情感交互的模式一个统计：哈哈哈哈，比如A对B比较友好，B对A当然哟好

![image-20220622090846571](https://s2.loli.net/2022/07/05/MtXYW1ZErThL4o8.png)

#### 模型缺点

ECM 的模型是在给出文本内容，同时给出你想要生成的回答的情感条件下，然后生成一句带有这个情感的回答。但是在日常对话中，并不会有上帝去给你指定要回复的情感。**情感应取决于主题、上下文或用户的情感。**

### 方向二：情感支持任务（ESConv 2021 等等）

什么是情感支持任务？根据用户的情感生成具有共情能力/开创性/有意义的回复

#### 数据集

Seeker Supporter mode

| 名称              | 解释                                                         | 特点   | 下载 |
| ----------------- | ------------------------------------------------------------ | ------ | ---- |
| ESConv（2021ACL） | 来访者-咨询师（心理治疗专家）模式，就是一个对话的数据集，里面都是专业的咨询师对对话的回复（1000个轮次 30/per）（40万rmb） | 质量高 |      |
|                   |                                                              |        |      |
|                   |                                                              |        |      |

### 论文ESConv：共情对话对话生成框架（2021）

#### 论文介绍

**这篇论文主要定义了情感支持对话的任务，并提出了一个电子稳定控制框架**(将心理学上的帮助技能理论改编成一个对话系统)

**主要任务：如何生成具有情感支持能力的回复**

#### 模型介绍

探索(探索以帮助寻求帮助者识别问题)

洞察(帮助寻求帮助者进入自我认识的新深度)

行动(帮助寻求帮助者做出应对问题的行动决定)

$$构建了一个情感支持对话数据集-$$

benchmark dataset *ESConv*

![image-20220622094037806](https://s2.loli.net/2022/07/05/976IaibzDTUYHgJ.png)

### 方向三：通过识别对话中的情绪原因提升共情回复生成



[Hanscal](https://www.zhihu.com/people/hanscal)

关注NLP领域，聚集于QA，对话和知识图谱。





论文题目：Improving Empathetic Response Generation by Recognizing Emotion Cause in Conversations[[1\]](https://zhuanlan.zhihu.com/p/508518264#ref_1)

代码地址：[https://github.com/A-Rain/EmpDialogue_RecEC](https://link.zhihu.com/?target=https%3A//github.com/A-Rain/EmpDialogue_RecEC)

这是哈工大、清华大学和悉尼大学合作研究发表于EMNLP-2021会议上的一篇论文，目前的移情反应生成方法侧重于学习一个模型来预先记录一个情绪标签，并根据这个标签生成回复，然而，情感原因是共情回复的一个基本因素，却被忽视了。情感起因是对人类情感的刺激。认识到情绪的原因有助于更好地理解人类的情绪，从而产生更多的同理心回复。为此，作者提出了一个新的框架，通过识别对话中的情绪原因来提高共情回复的生成。

### 论文CEM:常识推导+共情生成（2021）

#### 论文介绍

主要就是使得共情生成模型具备常识推导能力

**主要任务：如何理解用户对话，提出开创性的提议**

#### 具体结构

![image-20220622092823858](https://s2.loli.net/2022/07/05/HcSex3YTnANB2iW.png)



**上下文推导**

将对话历史中的上下文进行拼接，然后对每个 token 用向量表示，编码方式有 token embedding，position embedding 和 speaker embedding(或dialogue state embedding)。speaker embedding 用于区分不同的话语出自的说话者。接着将上下文矩阵输入编码器，得到上下文编码 

![image-20220622092926512](https://s2.loli.net/2022/07/05/AbLMZsRYHiUE8zg.png)

**知识获取**

对于一个输入序列将五个特殊的关系标记token加入到该序列后(CEM总览图左下部分表示)，然后利用 COMET 获得关于用户情况的不同角度的常识推理（上述的**五种推理**）。将**反应推理**结果作为**情感类**，其余推理结果作为**认知类**。对于情感类中的结果，输入编码器，再利用平均值池化，得到相应的**情感向量表示** ；对于认知类中的结果，输入编码器，再提取 [CLS] 对应的向量，得到相应的**认知向量表示** 。情感向量会经过一个线性层和 softmax，得到情感概率分布，于是利用交叉熵得到情感预测误差 。

![image-20220622093034569](https://s2.loli.net/2022/07/05/cjkQC87a2IuOsHw.png)

![image-20220622093022788](https://s2.loli.net/2022/07/05/5PMApbL9it2kDxH.png)

**上下文精炼**

两个独立的编码器(**情感精炼编码器**和**认知精炼编码器**)来融合的表示进行编码，并分别获得每个关系的**常识精炼后的上下文向量表示**，编码公式如下：

![image-20220622093228722](https://s2.loli.net/2022/07/05/5WhxJXK6FPuVqab.png)

#### 实验结果

人工评价和自动评价

评价指标分为**人工评价和自动评价。**作者采用了**困惑度(PPL)**和Distinct-n(Dist-n)作为主要的自动指标。

![image-20220622093120461](https://s2.loli.net/2022/07/05/aoejgc6Jy9AIt7h.png)

#### 数据集

Atomic  常识知识库用它做预训练的生成式模型 有COMET

### 论文MISC：知识图谱+混合策略+共情对话生成（2022）

Mixed Strategy for Emotional Support Emotional Support

#### 论文介绍

**主要任务：如何理解用户对话，提出开创性的提议***

MISC: A Mixed Strategy-Aware Model integrating COMET for Emotional Support Conversation**Emotion Understanding:*

如何基于多种不同策略，让机器在不同阶段和不同状态下选择具有引导性、且长期来看整体收益更高的策略

#### 模型介绍、

**第一个阶段**是**探索阶段**。这阶段我们需要询问去捕捉一些细节，同时了解用户当前情绪背后的诱因是什么。

第二个阶段是**安抚阶段**。在了解诱因后，我们需要通过情绪上的共鸣、通过自我披露来加深用户对我们的信任感。让用户觉得聊天机器人更有亲和力，从而更接纳它。

第三阶段是**建议阶段**。通过第二阶段的铺垫，我们才能在第三阶段的沟通中达到更好的效果，也让用户更愿意接受我们的建议，最终帮助到用户。

![image-20220622095853165](https://s2.loli.net/2022/07/05/DQgya7BS5ZKOzIn.png)

## 任务二 ：模板积累

目录

收起

背景介绍

模型结构

任务定义

情绪推理

回复生成

模型训练

实验部分

数据集

基线模型

实验结果

论文总结

# 共情对话生成领域

## 论文

其他论文

[[2106.01144\] Towards Emotional Support Dialog Systems (arxiv.org)](https://arxiv.org/abs/2106.01144)

[[2105.08316\] CoMAE: A Multi-factor Hierarchical Framework for Empathetic Response Generation (arxiv.org)](https://arxiv.org/abs/2105.08316)

[[2106.01702\] PsyQA: A Chinese Dataset for Generating Long Counseling Text for Mental Health Support (arxiv.org)](https://arxiv.org/abs/2106.01702)

[[2109.05739\] CEM: Commonsense-aware Empathetic Response Generation (arxiv.org)](https://arxiv.org/abs/2109.05739)

[[2110.08466\] On the Safety of Conversational Models: Taxonomy, Dataset, and Benchmark (arxiv.org)]

## 综述论文

看了一篇，考完试总结

## 我的论文报告

**COMET核心任务**

**Allen实验室发表在ACL2019的一篇关于自动常识知识库构建的文章。作者提出了Commonsense Transformers（COME）生成模型，主体框架是Transformer语言模型，在ATOMIC和ConceptNet知识库中选取种子知识训练集进行预训练，使得模型可以自动构建常识知识库。Allen实验室也提供了Demo和Code，Demo挺有意思的，输入一个event（有参与者），就可以返回一个常识知识图。**

**————————————————**

更具体地说，该问题假设COMET得到了{s, r, o}格式的自然语言元组训练知识库，其中s是元组的短语主题，r是元组的关系，o是元组的短语对象。例如，与“小睡”相关的ConceptNet元组是:(s=“小睡”，r=原因，o=“有精力”)。任务是生成o，在给定s和r作为输入的前提下。

我们定义Xs = {xs0 ……， x |s|}作为构成关系主题的标记，Xr = {xr0,……， xr|r|} 作为构成元组关系的标记，Xo = {xo0 . xr} 作为构成元组关系的标记，Xo = {xo0 . xr}作为构成元组关系的标记,……， xo|o|}作为组成元组对象的标记。任何单词x的嵌入都表示为e。

基于知识图谱再训练的transformer，生成新的三元组，补充原有的知识图谱。
[[共情对话系统调研]]

## 清华实验室公开资源colab

|                                                | 简介                                | 论文/代码                                                    | 其他                                                         |
| ---------------------------------------------- | ----------------------------------- | ------------------------------------------------------------ | ------------------------------------------------------------ |
| CDial-GPT 2020                                 | 模型：中文GPT                       | 论文/代码：https://arxiv.org/abs/2008.03946                                   https://github.com/thu-coai/CDial-GPT 预训练模型https://huggingface.co/thu-coai/CDial-GPT_LCCC-large | 有评测框架，文档太牛了好评                                   |
| MMChat 2022                                    | 模型：多模态对话系统                | 论文/代码:https://github.com/silverriver/MMChat    https://arxiv.org/abs/2108.07154 | ![image-20220505090640326](https://s2.loli.net/2022/07/05/qk5Q4cR8xBMnshN.png) |
| LCCC(Large-scale Cleaned Chinese Conversation) | 清洗脏话/颜文字的大型中文预训练框架 | 网盘：https://drive.google.com/file/d/1hhxXqEqmXegf8Ca0MVQyVshlEi7hsjPi/view?usp=sharing 介绍https://github.com/thu-coai/CDial-GPT | 对话轮次为百万级别，集合微博，百度文库的训练集合             |
| SentiLARE：用于情感分析的语言表示模型 2020     | 情感分析                            | 论文链接：https://www.aclweb.org/anthology/2020.emnlp-main.567/<br/><br/>代码、预训练模型、数据链接：https://github.com/thu-coai/SentiLARE                                        模型介绍：http://coai.cs.tsinghua.edu.cn/tools/4 | 引入词性和情感级性后适用于情感分析任务的语言表示模型         |

Towards Empathetic Open-domain Conversation Models: a New Benchmark and Dataset

MoEL：2019

[共情融合：](https://zhuanlan.zhihu.com/p/444190231)[MoEL](https://zhuanlan.zhihu.com/p/444190231)[: Mixture of Empathetic Listeners - ](https://zhuanlan.zhihu.com/p/444190231)[知乎 ](https://zhuanlan.zhihu.com/p/444190231)[(](https://zhuanlan.zhihu.com/p/444190231)[zhihu.com)](https://zhuanlan.zhihu.com/p/444190231)

**MIME:** **MIMicking** **Emotions for Empathetic Response Generation**

[情绪模仿：](https://zhuanlan.zhihu.com/p/444397424)[MIME: ](https://zhuanlan.zhihu.com/p/444397424)[MIMicking](https://zhuanlan.zhihu.com/p/444397424)[ Emotions for Empathetic Response Generation - ](https://zhuanlan.zhihu.com/p/444397424)[知乎 ](https://zhuanlan.zhihu.com/p/444397424)[(](https://zhuanlan.zhihu.com/p/444397424)[zhihu.com](https://zhuanlan.zhihu.com/p/444397424)[)](https://zhuanlan.zhihu.com/p/444397424)



多任务Transformer(Multi-TRS：2019）：Transformer的一种变体，有一个用于预测情绪的模块。联合优化NLL损失和用于情绪分类的交叉熵损失。

MoEL(2019)：一种基于Transformer的模型，对每个可能的用户情绪使用一个解码器，并将这些解码器的输出的表示柔和地组合起来以生成回复。因此，每个解码器都经过优化，以了解如何回复一种类型的情绪，而元解码器经过优化，以组合它们的表示并生成回复。

MIME(2020)：另一个基于Transformer的模型，在一定程度上模仿了检测到的用户情绪。在这种方法中，情绪分为消极和积极的情绪。该模型最初基于情绪组生成回复的模仿和非模仿表征，为了有效混合这些表征对模型进行优化，生成共情回复。

EmpDG(2020)：一种多分辨率对抗框架，由共情回复生成器和交互式判别器组成。生成器根据检测到的情绪生成共情回复，而鉴别器确保生成的回复与上下文一致，也具有同理心。为了与这篇论文中模型和其他基线进行公平比较，作者在实验中只实现了共情生成器，因为判别器需要来自对话中未来转折的信息。

![image-20220526111203968](C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20220526111203968.png)

![image-20220526110639349](https://s2.loli.net/2022/07/05/EH8BR2a5dblJSsN.png)



论文：AugESC: Large-scale Data Augmentation （明天搜）

###### 

数据集来源 : 高价购买 大约30-40万

数据条数：大约1000多轮对话

应对策略：

生成样例

![image-20220526110328582](https://s2.loli.net/2022/07/05/9wQaz8RLcSDdOyX.png)

数据增广

![image-20220526110104301](https://s2.loli.net/2022/07/05/RlFMkCUn4Av5zS6.png)

提出具有建设性的意见

![image-20220524003215402](https://s2.loli.net/2022/07/05/gbrdIT32xEKwtMf.png)

## 黄明烈老师交流会（学到挺多）



### 黄明烈老师论文分享会议

联系方式： 实验室/黄老师邮箱

![image-20220524002521013](https://s2.loli.net/2022/07/05/891vpyrXZqPKDx6.png)

黄老师实验室近期工作成果

![image-20220526113839229](https://s2.loli.net/2022/07/05/3exaTkUc18gXu5M.png)

其他论文

[[2106.01144\] Towards Emotional Support Dialog Systems (arxiv.org)](https://arxiv.org/abs/2106.01144)

[[2105.08316\] CoMAE: A Multi-factor Hierarchical Framework for Empathetic Response Generation (arxiv.org)](https://arxiv.org/abs/2105.08316)

[[2106.01702\] PsyQA: A Chinese Dataset for Generating Long Counseling Text for Mental Health Support (arxiv.org)](https://arxiv.org/abs/2106.01702)

[[2109.05739\] CEM: Commonsense-aware Empathetic Response Generation (arxiv.org)](https://arxiv.org/abs/2109.05739)

[[2110.08466\] On the Safety of Conversational Models: Taxonomy, Dataset, and Benchmark (arxiv.org)](https://arxiv.org/abs/2110.08466)

![image-20220526111645949](https://s2.loli.net/2022/07/05/mOjS9FTWHyGbJXL.png)

如何保证安全性（数据清洗，攻击识别）

![image-20220526111141425](C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20220526111141425.png)

数据增广

![image-20220526111254522](https://s2.loli.net/2022/07/05/iw9CjuO5Uhodsak.png)

###### Emohaa中文共情机器人

工作流 

**发现用户面临的问题**（情感计算/理解+领域知识）->**表达共情和理解**->**提出解决方案和建议（策略机制）->**进一步探索用户

Emohha的测试的例子

![image-20220526111422731](https://s2.loli.net/2022/07/05/JeKuXQkbAHBE6y2.png)

###### 子模块一：AugESC 使用大模型做数据增广，解决数据稀疏性问题

######  子模块二：建立对话安全性的评价标准，有一个评价体系

![image-20220526110920247](https://s2.loli.net/2022/07/05/DUuY9GQr3JApf1a.png)

**子模块三：处理用户恶意行为**

人在对话中并不期望明显的表露自己的状况信息和他们自己的感觉。但是，人可用自己的常识来理解这些显性的和隐性的表达。对话的双方会对对方的表达产生共情，对话系统也需要产生共情的回应，共情包含感情和认知两个方面，理性和情感对人类来说并不独立，在社交中情感通常是理性的。然而，当前对话模型仅关注其中一个方面，而忽视另外一个方面，导致回复无趣或不相关。除了识别用户的情感外，需要将用户的状况situation考虑进去。

2019年左右，一众研究者意识到了开放域对话系统具有共情能力的必要性

随后，通过两个独立的编码器(**情感精炼编码器**和**认知精炼编码器**)来融合的表示进行编码，并分别获得每个关系的**常识精炼后的上下文向量表示**，编码公式如下：

# 学习笔记

## **模型学习 &论文精读：transfomer**



### 对Transformer论文逐段精读

 姓名：陈可淇

学号：2019211955

### 精读动机

之前的学长的介绍使我对深度学习模型产生了浓厚的兴趣，于是我通过阅读相关论文并学习了深度学习领域中这三年出现的最具革命性的的模型Transformer。

题目：Attention is all your need

作者：

![image-20220619172956424](https://s2.loli.net/2022/07/05/UHPyLZ2Tt5N8vd4.png)

发表会议： NeurlPS2018

### 导言

#### rnn的局限和不足

![image-20220619002905885](https://s2.loli.net/2022/07/05/igDJ47AQl9vcK3I.png)

因为rnn是经典的时序神经网络，RNN根一个序列的隐藏转态$$h_{t-1}$$和$$t$$时刻的输入生成这个状态的隐藏状态。如下图

这样会导致一系列问题，例如无法并行，梯度爆炸（消失）等等，当然有LSTM GRU等模型出现，不过治标不治本

优势：transformer使用的是注意力机制，与时序无关，相对RNN使得模型能够获得并行训练的效果。

#### CNN的优势与不足



cnn是卷积神经网络，其特点是将一个使用一个卷积窗口获取像素及其周边的像素块。其优势是更够获取多通道的信息，但是其局限是如果要获取两个相邻较远的像素块的话，需要叠加多层CNN。

优势：transformer采取的是注意力机制，其能够在一句话中获取所有词的信息，而transformer又因为使用（multi-head）多头注意力机制，其也能像CNN一样获取多输出通道的效果。

### transformer模型分析



#### encoder-decoder架构

encoder的输入是一序列的符号表示$$(x_{1},....x_{n})$$ ，输出是一段连续的标识z=$$(z_{1},...,z_{n})$$,

decoder的输入为z，生成的是$$(y_{1},...,y_{m})$$,值得注意的是N！=m

encoder的生成式自回归的，简单的来说是根据$$y_{1}生成y_{2}$$….

图

 ![image-20220619003113606](https://s2.loli.net/2022/07/05/ugyYRmPnW56qcE1.png)





#### 模型架构（图）详细解释

编码器解码器

![image-20220619171828135](https://s2.loli.net/2022/07/05/AOeUVyMgR5T8PCj.png)

另外一种画法

![image-20220619152241654](https://s2.loli.net/2022/07/05/l5SDuB3OhoYR6AX.png)

#### 什么是自注意力机制

我们通过几个步骤来解释：

注意力机制的位置：

![image-20220619152952133](https://s2.loli.net/2022/07/05/cHzC8WX1aAfnESm.png)

自注意力的公式：如下



![image-20220619153129783](https://s2.loli.net/2022/07/05/aFU4vo3NBgh8CSd.png)

下面图解上述公式：

1、首先，self-attention的输入就是词向量，即整个模型的最初的输入是词向量的形式。那自注意力机制呢，顾名思义就是自己和自己计算一遍注意力，即对每一个输入的词向量，我们需要构建self-attention的输入。在这里，transformer首先将词向量乘上三个矩阵，得到三个新的向量，之所以乘上三**个矩阵参数**而不是直接用原本的词向量是因为这样增加更多的参数，提高模型效果。对于输入X1(机器)，乘上三个矩阵后分别得到Q1,K1,V1

![image-20220619153256086](https://s2.loli.net/2022/07/05/E1UrISnReZV34Mt.png)





![image-20220619153129783](https://s2.loli.net/2022/07/05/aFU4vo3NBgh8CSd.png)

2 那接下来就要计算注意力得分了，这个得分是通过计算Q与各个单词的K向量的点积得到的。我们以X1（x矩阵的第一列）为例，分别将Q1和K1、K2进行点积运算，假设分别得到得分112和96。（$$QK^{t}$$）点乘

![image-20220619162152887](https://s2.loli.net/2022/07/05/BN85RKylId72hLi.png)

3、将得分分别除以一个特定数值8（K向量的维度的平方根，通常K向量的维度是64）这能让梯度更加稳定（$${QK^{t}}/\sqrt{d_{k}}$$）

4、将上述结果进行softmax运算得到，softmax主要将分数标准化，使他们都是正数并且加起来等于1。（Softmax（$${QK^{t}}/\sqrt{d_{k}}$$）） 得到0.88和0.12

![image-20220619160925008](https://s2.loli.net/2022/07/05/djoIfEqGiYmrZB4.png)

5、将V向量乘上softmax的结果，这个做法主要是为了保持我们想要关注的单词的值不变，而掩盖掉那些不相关的单词（例如将他们乘上很小的数字）

$$Softmax（{QK^{t}}/\sqrt{d_{k}}）V$$

![image-20220619162717805](https://s2.loli.net/2022/07/05/FxMhkIgKEONToDr.png)

6、将带权重的各个V向量加起来，至此，产生在这个位置上（第一个单词）的self-attention层的输出，其余位置的self-attention输出也是同样的计算方式。

![image-20220619163012959](https://s2.loli.net/2022/07/05/bNC5dwfcRLZlaPo.png)

**总结：自注意力的本质就是把输入词向量用不同的W分成query(Q)，key(K)和value(K)三个部分。Q和K相乘可以看作一个retrieval的过程，Q是查询要求，K是候选结果的title，V是候选结果的具体内容。每个单词的Q和所有其他单词的K做匹配，看和各个单词的相关程度（单词的向量相似度）（也就是softmax得到的概率），这个相关程度去和每个单词的V做weighted sum，从各个单词中根据需要提取信息。**

### 为什么用自注意力机制？

![image-20220619170127451](https://s2.loli.net/2022/07/05/eB79nSaExcQWpvt.png)

这三个指标的含义

Complexity  per layer : 计算复杂度

Sequential Operation: 顺序计算（下一步计算需要等前面多少个计算？）（可并行度高）

Maximum Path Length: 节点到节点的信息传递距离（越短越好）

可见由于自注意力结构信息传递距离为1（），可并行度高

相比RNN和CNN都较好，

#### 结果和实验细节



![image-20220619171509820](https://s2.loli.net/2022/07/05/gLIJyVPHXbxjwqa.png)



自动变换学习率的操作

![image-20220619171613195](https://s2.loli.net/2022/07/05/js1XYS2BVxTt7ku.png)

#### 超参数（比较简洁）

N：子层的数量

d_model: dimension的数量

h：多少个头

![image-20220619171949426](https://s2.loli.net/2022/07/05/8IikDJ59fzm6hXU.png)

### 读论文总结

总而言之，attention的作用就是吧序列中的所有信息汇聚起来，把它加工成所需要的信息。

Transformer结构图，传递信息的方式，几乎能用在几乎所有的NLP,CV任务上，transformer深刻影响了近3年的的AI论文

趋势：

tranformer+多模态

可解释性

attention序列化

![image-20220619165503120](https://s2.loli.net/2022/07/05/f7OT6o1MrcF9wWX.png)

特点调参简单，只有两个参数

rnn传递信息的方式

![image-20220619165450683](https://s2.loli.net/2022/07/05/qNLwDKpOTEfzj28.png)



### 英文写作

#### **特点：**

简洁，没有太多的写作技巧

讲一个故事

#### 论文中英文句式的积累

For our base models using the hyperparameters described throughout the paper, each training step took about 0.4 seconds.

**To best of our knowledge,however**,the Transformer is first transduction model relying entirely on self-attention to compute representations of its input and output without using sequence-aligned RNN or convolution.

As each step the model i

## **模型学习：GPT3（主要是使用）**

### GPT-3

key - 的申请

#### 深度学习-Pre-training-fine-toning

简单介绍GPT-3

每个Transformer单元相当于一层的RNN层，接收一整个句子所有词作为输入，然后为句子中的每个词都做出一个输出。但是与RNN不同的是，Transformer能够同时处理句子中的所有词，并且任意两个词之间的操作距离都是1，这么一来就很好地解决了上面提到的RNN的效率问题和距离问题。

每个Transformer单元都有两个最重要的子层，分别是Self-Attention层与Feed  Forward层，后面会对这两个层的详细结构做介绍。文章使用Transformer搭建了一个类似Seq2Seq的语言翻译模型，并为Encoder与Decoder设计了两种不同的Transformer结构。

GPT-3和bert 的差别

| GPT-3            | BERT                                   |
| ---------------- | -------------------------------------- |
| Transfomer编码器 | 解码器                                 |
| 单向             | 双向                                   |
|                  | mask                                   |
|                  | 都是transformer的+pretrain+fine tuning |
| BPE(字节码)      |                                        |

### 预训练(pre-training/trained)：

你需要搭建一个网络来完成一个特定的图像分类的任务。首先，你需要随机初始化参数，然后开始训练网络，不断调整直到网络的损失越来越小。在训练的过程中，一开始初始化的参数会不断变化。当你觉得结果很满意的时候，就可以将训练模型的参数保存下来，以便训练好的模型可以在下次执行类似任务时获得较好的结果。这个过程就是pre-training。

之后，你又接收到一个类似的图像分类的任务。这个时候，你可以直接使用之前保存下来的模型的参数来作为这一任务的初始化参数，然后在训练的过程中，依据结果不断进行一些修改。这时候，你使用的就是一个pre-trained模型，而过程就是fine-tuning。

所以，预训练就是指预先训练的一个模型或者指预先训练模型的过程；微调 就是指将预训练过的模型作用于自己的数据集，并参数适应自己数据集的过程。

### 微调的作用

在CNN领域中。很少人自己从头训练一个CNN网络。主要原因上自己很小的概率会拥有足够大的数据集，从头训练，很容易造成过拟合。

所以，一般的操作都是在一个大型的数据集上训练一个模型，然后使用该模型作为类似任务的初始化或者特征提取器。比如VGG，Inception等模型都提供了自己的训练参数，以便人们可以拿来微调。这样既节省了时间和计算资源，又能很快的达到较好的效果。 

大家好，我是19级软件工程专业的陈可淇，有过半年左右轨迹预测方向的科研经历，计划在实验室实习的方向是口语对话系统，请大家多多指教~~

我这周还是在做轨迹预测方向的事情，那边目前还是顺利的，ddl是5月17号（CIKM） 应该可以赶上，然后17号之后我可以花大多数时间在这边的工作了。

不中就转期刊

口语对话系统方向的话，我就到github上找了一些主流模型，看了一下源码，还没部署。

GAN 论文

类型、

![image-20220428122852193](https://s2.loli.net/2022/07/05/BGEOdFDelujLzJo.png)

## **工具学习：RASA(没啥用)**

Rasa是一个基于多轮对话的框架，其中包含两个模块Rasa core与Rasa nlu。

**Rasa nlu**是用来理解语义的，包括意图识别，实体识别，它会把用户的输入转换为结构化的数据，例如在下图的例子中，nlu会识别出用户打算发一封邮件（意图），邮箱地址amy@example.com（实体）。Rasa Core是一个对话管理的平台，它的工作是决定接下来机器该返回什么内容给用户，这里给用户返回了Should we make that your primary email?

Tokenize->Featurize->NER Extract->Intent Classify  大概流程吧

![image-20220616121600863](https://s2.loli.net/2022/07/05/OvMIaXLdNx89HmG.png)

![image-20220428113605250](https://s2.loli.net/2022/07/05/Xp3yUYhRSeWtkEP.png)

**Rasa Core**是一个对话管理的平台，它的工作是决定接下来机器该返回什么内容给用户，这里给用户返回了Should we make that your primary email?

![image-20220428111512502](https://s2.loli.net/2022/07/05/4HaAGIdSCBtu6UQ.png)

![image-20220428113257560](https://s2.loli.net/2022/07/05/MK1Ibl9LDPFQOYi.png)

### NLU

NLU的任务是解析消息，它能把自然语言解释成我们需要的结构化的数据，我们继续完善下去。

NLU的任务是解析消息，它能把自然语言解释成我们需要的结构化的数据，我们继续完善下去。

可以设置多个机器人，可以面向不同领域

![image-20220428110735512](https://s2.loli.net/2022/07/05/SR81MXsNqvdi9l6.png)

![image-20220428111702800](https://s2.loli.net/2022/07/05/Xm8NAZp17gPGsfT.png)

1. 支持命令行启动训练和推理
2. 支持http调用，并满足统一的接口规范
3. 支持训练数据和模型远程存储

### RASA信息流向

1. 消息传入后，被Interpreter接收
2. interpreter接收消息后，将消息转换成字典（tokenizer），并转化成特征（featurizer），提取命名实体（Extractors），识别意图（Classifier）。这部分叫做自然语言理解（NLU）。interpreter将输出包括实体，意图，以及对话的特征一起传给Tracker。
3. Tracker用来追踪记录对话状态的对象，Tracker的当前状态（特征，意图，实体）以及历史状态信息一并传给Policy。
4. Policy将当前状态以及历史状态一并特征化，并传入预测模型（Policy），预测模型预测出下一个动作（Action）。
5. Action完成实际动作，并将动作结果通知到tracker，成为历史状态。
6. Action将结果返回给用户。

### 扩展：

意图分类器

实体提取器

### Rasa大佬连接     https://zhuanlan.zhihu.com/p/331806270

Rasa为建立高效，灵活，专有的上下文对话机器人提供了必要的基础架构和工具。使用Rasa，任何人员都可以通过文本编辑器配置配置文件，就可以得到一个非常不错的对话机器人。

正因为对话机器人有如此广泛的应用，技术应用也层出不穷。如百度开源的基于检索式机器人的框架AnyQ；Google开源的基于生成式对话系统DeepQA；Facebook开源的基于阅读理解的系统DrQA；北京大学知识库问答系统gAnswer。但这些技术都是为了完成对话系统中的一个任务，或者说为了机器人的一个能力而开发的技术，而现有的对话系统中多是各种技术的混合，例如一个对话系统，闲聊部分可能用到DeepQA一类的NLG技术，关于知识推理部分可能用到KBQA的部分，关于FAQ的回答可能用到AnyQ或者DRQA。如何将这些技术应用到一个系统中，还是对应用开发人员的一个考验。

幸运的是，近些年来，很多厂商都开源了自己的问答系统，整个系统是开包即用，例如Facebook开源的Blender系统，他具有个性人物聊天的功能，可以知识问答，是有史以来最大的开放域（Open-Domain）聊天机器人。还有Uber开源的Plato系统，也都具有比较完整的功能。但要说从**框架完整性，可扩展性，易用性**等各方面，RASA当仁不让是当前最全面的系统之一。下面我们详细介绍下RASA系统。

#### 1、Stories

stories可以理解为对话的场景流程，我们需要告诉机器我们的多轮场景是怎么样的，例如，在下文的例子中，我们希望的流程是这样的：用户问好 -> 机器问用户今天过得怎么样 -> 用户反馈情绪 -> 机器根据不同的情绪进行回复，这里其实包含两个流程，一个正面情绪的流程与一个负面情绪的流程，因此，我们也需要编写两个story，接下来我们看下怎么编写story。
符号 	说明

![image-20220428111155378](C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20220428111155378.png)

story 标题

* 	意图

- 动作

  2、Domain

  domain可以理解为机器的知识库，其中定义了意图，动作，以及对应动作所反馈的内容。

# 资源

## 其他开源数据  NLP

|                                              | 简介                               | 代码/论文/网盘                                               | 其他                           |
| -------------------------------------------- | ---------------------------------- | ------------------------------------------------------------ | ------------------------------ |
| STC 数据集  权威                             | 公开数据集比较有名，论文中出现较多 | train/test https://drive.google.com/file/d/1jsTyvOz0y_6UIAkaibvvxf6bw0REqAlO/view?usp=sharing test https://drive.google.com/file/d/15jEriASrMX4r1zShY-pvDPLt-gOF4Wbg/view?usp=sharing | 大家都在用，好像是2017的       |
| CMDA （不权威）                              | 中文医疗数据集                     | https://github.com/Toyhom/Chinese-medical-dialogue-data      | 逛github看到的，但是感觉比较拉 |
| Cornell Movie Dialogs 权威（下载网址不确定） | 康奈尔的电影对话                   | https://download.csdn.net/download/u014736221/10596024?spm=1001.2101.3001.6661.1&utm_medium=distribute.pc_relevant_t0.none-task-download-2%7Edefault%7ECTRLIST%7EPaid-1.pc_relevant_default&depth_1-utm_source=distribute.pc_relevant_t0.none-task-download-2%7Edefault%7ECTRLIST%7EPaid-1.pc_relevant_default&utm_relevant_index=1 | 2M影评数据集，究极老的数据集   |
|                                              |                                    |                                                              |                                |
| 中文词向量                                   | （不威）                           | 腾讯10G（本地）、https://github.com/fighting41love/funNLP、gia |                                |
| 中文聊天语料库 不                            | （权威）                           | https://github.com/codemayq/chaotbot_corpus_Chinese          | 豆瓣，青云语料，电视剧对白     |
| 中文问答数据集                               | （不权威）                         | https://pan.baidu.com/s/1QUsKcFWZ7Tg1dk_AbldZ1A              | 没看                           |
| 对联数据23333                                |                                    | https://github.com/wb14123/couplet-dataset                   |                                |
| 青云语料库                                   | 权威                               | 但是没有                                                     |                                |
| 大规模医疗对话集                             |                                    | https://github.com/yaleimeng/Final_word_Similarity           | 110万条医学咨询                |
| 根据rasa对话的代码                           | rasa速速参考                       | https://github.com/GaoQ1/rasa_chatbot_cn                     | 下周                           |

竟然可以在外包平台上进行人工评测来验证机器生成的对话，牛啊

## 辅助任务：知识图谱：情感分析：非对话的中文语料

|                                          | 简介       | 资源                                                    | 其他 |
| ---------------------------------------- | ---------- | ------------------------------------------------------- | ---- |
| 中文事件抽取                             | 事件抽取   | https://github.com/liuhuanyong/ComplexEventExtraction   |      |
|                                          |            |                                                         |      |
| 清华的跨语言知识图谱                     | 知识图谱   | https://xlore.org/download.html                         |      |
| 微信公众号爬虫的结果                     | 不如自己爬 | https://github.com/nonamestreet/weixin_public_corpus    |      |
| 苏大的句法标注                           |            | http://hlt.suda.edu.cn/index.php/Nlpcc-2019-shared-task |      |
| 瑞金医院知识图谱                         |            | https://github.com/geekinglcq/CDCS                      |      |
| 2015年至19年的所有kaggle上的知识图谱数据 | 权威       | https://github.com/geekinglcq/CDCS                      |      |
| 中文知识图谱的资源汇总                   |            | https://github.com/husthuke/awesome-knowledge-graph     |      |
| 中文知识图谱汇总                         |            | https://github.com/husthuke/awesome-knowledge-graph     |      |
| 中文词语相似度                           |            | https://github.com/yaleimeng/Final_word_Similarity      |      |

|                                |                                                              | 资源                                                         |
| ------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ |
| 知识图谱                       | 小综述                                                       | https://developer.aliyun.com/article/761513?utm_content=g_1000124809 |
| 132知识图谱数据集              | 常识、城市、金融、农业、地理、气象、社交、物联网、医疗、娱乐、生活、商业、出行、科教啊啊啊太多了 | http://openkg.cn/dataset                                     |
|                                |                                                              |                                                              |
| 维基百科，百度百科             |                                                              | https://gist.github.com/thomwolf/13ca2b2b172b2d17ac66685aa2eeba62 |
| 大规模中文知识图谱             | 1.3亿实体                                                    | https://github.com/ownthink/KnowledgeGraphData               |
|                                | 序列标注工具                                                 | http://brat.nlplab.org/index.html                            |
| 人民日报语料库                 |                                                              | https://github.com/howl-anderson/tools_for_corpus_of_people_daily |
| 句子相似度判定模型             |                                                              | https://github.com/liuhuanyong/SiameseSentenceSimilarity     |
| 基于医药知识图谱的智能问答系统 |                                                              | https://github.com/YeYzheng/KGQA-Based-On-medicine           |

NePF方向的

https://github.com/yenchenlin/awesome-NeRF

## 瑞士军刀:学习资料

|                        | 解释             | 资源                                                  |
| ---------------------- | ---------------- | ----------------------------------------------------- |
| jieba                  | 不多bb           |                                                       |
| 复旦NLP                | 复旦nlp集        | https://github.com/fighting41love/funNLP              |
|                        |                  | https://github.com/nl8590687/ASRT_SpeechRecognition   |
| 命名实体               | 之前有搜集了一堆 |                                                       |
| 三元组搜取             |                  | https://github.com/liuhuanyong/EventTriplesExtraction |
| 啊啊太多了用的时候再找 |                  |                                                       |
|                        |                  | https://github.com/huyingxi/Synonyms                  |
| 真得供起来烧柱香       |                  | https://github.com/fighting41love/funNLP              |
| 清华2018年的报告       | ybb              | https://static.aminer.cn/misc/article/nlp.pdf         |
| 自然语言的基本模型     |                  | https://github.com/lpty/nlp_base                      |

学习

https://github.com/npubird/KnowledgeGraphCourse



 **ASR 语音数据集 + 基于深度学习的中文语音识别系统：**  [github](https://github.com/nl8590687/ASRT_SpeechRecognition)

- Data Sets 数据集

  - **清华大学THCHS30中文语音数据集**

    data_thchs30.tgz [OpenSLR国内镜像](http://cn-mirror.openslr.org/resources/18/data_thchs30.tgz) [OpenSLR国外镜像](http://www.openslr.org/resources/18/data_thchs30.tgz)

    test-noise.tgz [OpenSLR国内镜像](http://cn-mirror.openslr.org/resources/18/test-noise.tgz) [OpenSLR国外镜像](http://www.openslr.org/resources/18/test-noise.tgz)

    resource.tgz [OpenSLR国内镜像](http://cn-mirror.openslr.org/resources/18/resource.tgz) [OpenSLR国外镜像](http://www.openslr.org/resources/18/resource.tgz)

  - **Free ST Chinese Mandarin Corpus**

    ST-CMDS-20170001_1-OS.tar.gz [OpenSLR国内镜像](http://cn-mirror.openslr.org/resources/38/ST-CMDS-20170001_1-OS.tar.gz) [OpenSLR国外镜像](http://www.openslr.org/resources/38/ST-CMDS-20170001_1-OS.tar.gz)

  - **AIShell-1 开源版数据集**

    data_aishell.tgz [OpenSLR国内镜像](http://cn-mirror.openslr.org/resources/33/data_aishell.tgz) [OpenSLR国外镜像](http://www.openslr.org/resources/33/data_aishell.tgz)

  注：数据集解压方法

  ```
  $ tar xzf data_aishell.tgz
  $ cd data_aishell/wav
  $ for tar in *.tar.gz;  do tar xvf $tar; done
  ```

  - **Primewords Chinese Corpus Set 1**

    primewords_md_2018_set1.tar.gz [OpenSLR国内镜像](http://cn-mirror.openslr.org/resources/47/primewords_md_2018_set1.tar.gz) [OpenSLR国外镜像](http://www.openslr.org/resources/47/primewords_md_2018_set1.tar.gz)







# 组会笔记

## 每周周记

| 工作整体计划 | 应填写最近工作的整体目标、工作内容和时间安排     需列出每一项工作内容完成的时间节点，即Milestone。 | 工作整体计划完成情况 |      | 应填写到目前为止已经完成的全部工作，须对照左侧工作计划逐项填写。如未完成请估计完成的百分比。 |
| ------------ | ------------------------------------------------------------ | -------------------- | ---- | ------------------------------------------------------------ |
| 开始打工     | 调研了微软的RASA                                             | 没啥用               |      | 研究黄老师的工作                                             |
|              | 完成轨迹预测的论文，究极折磨                                 |                      |      |                                                              |
|              | 看了colab的github                                            |                      |      |                                                              |
|              |                                                              |                      |      |                                                              |
|              |                                                              |                      |      |                                                              |



| 工作整体计划 | 应填写最近工作的整体目标、工作内容和时间安排     需列出每一项工作内容完成的时间节点，即Milestone。 | 工作整体计划完成情况 |      | 应填写到目前为止已经完成的全部工作，须对照左侧工作计划逐项填写。如未完成请估计完成的百分比。 |
| ------------ | ------------------------------------------------------------ | -------------------- | ---- | ------------------------------------------------------------ |
|              | 听了周五情感计算的汇报,写了一个组会的总结50%，感觉听会议比看综述有用多了 | 然鹅没录上音         |      | 准备下周组会ppt                                              |
|              | COMET的论文                                                  |                      |      | 下周组会讲COMET                                              |
|              | CDial-GPT 2020论文                                           |                      |      |                                                              |
|              | AugESC ：使用大模型做数据增广                                |                      |      |                                                              |
|              |                                                              |                      |      |                                                              |



| 工作整体计划 | 应填写最近工作的整体目标、工作内容和时间安排     需列出每一项工作内容完成的时间节点，即Milestone。 | 工作整体计划完成情况 |      | 应填写到目前为止已经完成的全部工作，须对照左侧工作计划逐项填写。如未完成请估计完成的百分比。 |
| ------------ | ------------------------------------------------------------ | -------------------- | ---- | ------------------------------------------------------------ |
|              | 准备组会ppt                                                  |                      |      |                                                              |
|              | 看了和COMET有关的几篇论文                                    |                      |      | ACL 2022 C3KG：https://github.com/XiaoMi/C3KG<br/>ACL 2022 MISC: https://github.com/morecry/MISC<br/>SIGIR 2021 Emma: https://github.com/XiaoMi/emma |
|              | 调研了Emohha,对比了小冰                                      |                      |      |                                                              |
|              | 听了周末智源的报告 ！收获很多！                              |                      |      |                                                              |
|              |                                                              |                      |      |                                                              |

## 开始放假

**放假第一周**

| 本周工作整体计划 | 应填写最近工作的整体目标、工作内容和时间安排     需列出每一项工作内容完成的时间节点，即Milestone。 | 下一周工作整体计划完成情况 | 应填写到目前为止已经完成的全部工作，须对照左侧工作计划逐项填写。如未完成请估计完成的百分比。 |
| ---------------- | ------------------------------------------------------------ | -------------------------- | ------------------------------------------------------------ |
|                  | 期末！                                                       | 30%                        | 调研报告                                                     |
|                  |                                                              |                            | 综合多篇论文准备组会报告                                     |
|                  |                                                              |                            | ACL 2022 MISC: https://github.com/morecry/MISC               |
|                  |                                                              |                            | ACL 2022 C3KG：https://github.com/XiaoMi/C3KG<br/>ACL 2022 MISC: https://github.com/morecry/MISC<br/>SIGIR 2021 Emma: https://github.com/XiaoMi/emma |

**放假第二周**

| 本周工作整体计划 | 应填写最近工作的整体目标、工作内容和时间安排     需列出每一项工作内容完成的时间节点，即Milestone。 | 下一周工作整体计划完成情况 | 应填写到目前为止已经完成的全部工作，须对照左侧工作计划逐项填写。如未完成请估计完成的百分比。 |
| ---------------- | ------------------------------------------------------------ | -------------------------- | ------------------------------------------------------------ |
|                  | 期末！                                                       | 50%                        | 调研报告零完成，开始写调研报告一                             |
|                  | 周二考完试，开始写综述                                       |                            |                                                              |
|                  | 阅读完成这四个篇论文  ACL 2022 C3KG：https://github.com/XiaoMi/C3KGACL 2022 MISC: https://github.com/morecry/MISCSIGIR 2021 Emma: https://github.com/XiaoMi/emma ACL 2022 MISC: https://github.com/morecry/MISC |                            |                                                              |
|                  | 看了沙河超算介绍会议，写了一个使用沙河超算的文档             |                            |                                                              |
|                  | 李沐课程                                                     |                            |                                                              |

**放假第三周**（X）

| 本周工作整体计划 | 应填写最近工作的整体目标、工作内容和时间安排     需列出每一项工作内容完成的时间节点，即Milestone。 | 下一周工作整体计划完成情况 | 应填写到目前为止已经完成的全部工作，须对照左侧工作计划逐项填写。如未完成请估计完成的百分比。 |
| ---------------- | ------------------------------------------------------------ | -------------------------- | ------------------------------------------------------------ |
|                  | 整合所有论文阅读笔记，完善第二份调研报告                     | 80%                        | 调研报告收尾                                                 |
|                  | 整理笔记                                                     |                            | 复现论文MISC                                                 |
|                  | 李沐课程                                                     |                            | 复现论文CEM                                                  |
|                  |                                                              |                            | 动手构建共情对话系统，先画一个框架图                         |

## 王学长讲英文论文写作中注意的事项

英文写作

60个词太长

转换为列表的形式

![image-20220616093453216](https://s2.loli.net/2022/07/05/xltM8pwFWVSAdHu.png)

、![image-20220421101124637](https://s2.loli.net/2022/07/05/puotDJci9yRjMIW.png)

强调

中国学生在英文写作中的问题

![image-20220616094704130](https://s2.loli.net/2022/07/05/mFo8JvQhlbgs1iE.png)

上海纽约大学的一个教授讲的

![image-20220616093559143](https://s2.loli.net/2022/07/05/7ginZrxFLCBoPHk.png)

This paper



![image-20220616093640021](https://s2.loli.net/2022/07/05/1e6gSlNu9U3Ecvq.png)

which和that需要指代明确

驶入没有逗号，容易被人误认为形容后面那个词

![image-20220616093802894](C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20220616093802894.png)

这个词应该有强烈的对比意味

![image-20220616093911723](C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20220616093911723.png)



![image-20220616093947660](https://s2.loli.net/2022/07/05/r6j1IVfEgszCKqG.png)

错误：滥用

无意义的

![image-20220616094002792](https://s2.loli.net/2022/07/05/Svj58Atr4dJEfUK.png)

In this paper 

in this study



![image-20220616094022051](https://s2.loli.net/2022/07/05/xZWejDAp9ml7Vw5.png)

in this study

![image-20220616094126509](C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20220616094126509.png)



![image-20220616094157589](C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20220616094157589.png)

避免使用阿拉伯数字，（真的高傲！），阿拉伯数字小于等于10的话，尽量使用英文数字

![image-20220616094211802](C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20220616094211802.png)

greater than

![image-20220616094301910](https://s2.loli.net/2022/07/05/K3zhasIMHXw8pQx.png)

用在末尾表示列表没有结束，同时使用冗余

![image-20220616094336833](https://s2.loli.net/2022/07/05/GFSecgn1jWVAbBd.png)

如果表达完整的话，用下面的那个比较好

![image-20220616094432928](https://s2.loli.net/2022/07/05/6Jv9RdiknaXpfqK.png)

缩写尽量不要写在句子的开头，不要用in 需要as

![image-20220616094512113](https://s2.loli.net/2022/07/05/WspbftzyBmFNrUL.png)

如果要表示国界使用China

![image-20220616094624162](https://s2.loli.net/2022/07/05/LPTAzMi2ZwBnpyE.png)

英文引用后面加空格



比较的时候

不能说这个系统好于那个指标，就是比较的时候要说

这个系统的这个指标好于那个指标



美式英语和英式英语

格式会有latex模板

国外的一个教授经常收到垃圾邮件，所以写了这篇文章。格式

![image-20220616094851368](https://s2.loli.net/2022/07/05/zpxJM8COSL2wD1G.png)

## 组里讲工具

![image-20220616094907940](https://s2.loli.net/2022/07/05/ZwELY1obBu8Id2O.png)



资源

找到一篇文章及其相关量的文章

![image-20220616095123316](https://s2.loli.net/2022/07/05/2AjU9QSNp7W5s4m.png)

![image-20220616095050532](https://s2.loli.net/2022/07/05/UurJxZPSlz9dDci.png)

VPN网站

90块用一年

![image-20220616095221610](https://s2.loli.net/2022/07/05/QBVEKI4MxnzNCw7.png)

找文章

![image-20220616095336866](https://s2.loli.net/2022/07/06/QwImXHWj6vF5PkC.png)

AI写作助手 付费的

![image-20220616095449188](https://s2.loli.net/2022/07/06/rik2dawObxWsNUy.png)

![image-20220616095408962](https://s2.loli.net/2022/07/06/5TSdaInBAfc7vpy.png)

动手学深度学习Pytorch版

JUpyter lab 使用Xshell超级方便

李沐

付费版，word李沐可以用这个插件

Snipaste+按下F1就可以截图其实就是那个鼠标界面截图

一个

这些尽量都装

![image-20220616100405150](https://s2.loli.net/2022/07/06/FH7ZxBUl4LNbKTP.png)

截屏软件

![image-20220616095623150](https://s2.loli.net/2022/07/06/MeJP89viFWcphkS.png)

![image-20220616100548979](https://s2.loli.net/2022/07/06/E3hCQfZus25wS7B.png)

![image-20220616095610195](https://s2.loli.net/2022/07/06/TAHQl5iusOMWkLy.png)

Utools 按住Utools+空格忽然想做笔记 MD

Snipaste

如果看论文没有合适的阅读器

![image-20220616095734841](https://s2.loli.net/2022/07/06/BuyVQCvwF3xUoRe.png)

查看词频

![image-20220616100758851](https://s2.loli.net/2022/07/06/CLYMcRAe6jStZqE.png)

![image-20220616100846404](https://s2.loli.net/2022/07/06/szWvRAxuSt6IHgC.png)

有多种表达方式，但是你不知道哪个更符合应用

Total Commander windows下的资源管理器，会很慢

你类似使用LINUX WINDOWS

文本 比较工具（非word工具）

小工具：wiki上有

warn

文本编辑，空格差异

全文搜索工具

file locator

比如文件内的某个字符或者文字

![image-20220616110158439](https://s2.loli.net/2022/07/06/j1YnQMuiUND79zo.png)



![image-20220616100810853](https://s2.loli.net/2022/07/06/FqDC69QMJ2wItnW.png)

google

梯子 墙内能访问

tapfog

![image-20220616101101499](https://s2.loli.net/2022/07/05/DGROQthwHXVFrqb.png)

![image-20220616103146913](https://s2.loli.net/2022/07/05/3o5svLQtqK7SNAc.png)

熊老师推荐

学长推荐：智源社区

![image-20220616110343044](https://s2.loli.net/2022/07/05/gIbtxa3V5MXrluR.png)

## 学姐的论文审稿意见

做的工作要一致：

这个图一开始应该这么画，后来应该这么画

前变量训练模型对mask解码进行后验证分布

![image-20220616105938215](https://s2.loli.net/2022/07/05/sSFVoAi23EH7wlq.png)

![image-20220616105902510](https://s2.loli.net/2022/07/05/kHDGvdy3jahNfCY.png)



邓学姐投出的Inter speech审稿意见

语音合成的基础知识，基础一定要牢固（要学），如何去提高，要看综述

![image-20220616111448714](https://s2.loli.net/2022/07/05/mJ1GxQ4XyVqTekH.png)

眨眼

![image-20220616110754412](https://s2.loli.net/2022/07/05/rf4TgpS2HA8aXwL.png)

![image-20220616110734629](https://s2.loli.net/2022/07/05/mHYgdG4FiCMhnok.png)

![image-20220616111403343](https://s2.loli.net/2022/07/05/E7L5SiV9HZorFcj.png)

## 高老师讲论文评审工作



高老师讲论文评审工作hhh

不要自己说服自己！！！！

要从别人的角度看待，比如从最基础的概念开始！解释，专家可能不懂，审稿，审稿意见，仔细的去看看别人的论文，帮你在另外一个维度思考问题。

![image-20220616122019479](https://s2.loli.net/2022/07/05/aICiAObkQtB5X7K.png)

访问committee

![image-20220616121833598](https://s2.loli.net/2022/07/05/WNhpz3nEZ5FTar7.png)

会有一个申诉机制，评审专家的申诉hhh

![image-20220616122147623](https://s2.loli.net/2022/07/05/sIvQLmYdaK9iPyR.png)

# 写论文笔记

## 腾讯文档

[destination predication (qq.com)](https://docs.qq.com/sheet/DZElLdlZtRUJtZ3hI?scene=027a498772f23c44b1ee4b637uwCn1&tab=BB08J2)

## Scihub

[Sci-Hub: removing barriers in the way of science](https://sci-hub.st/)

https://sci-hub.st/

## 序号：读论文的模板

![](https://s2.loli.net/2022/07/05/2CE8X3A7wPno1dJ.png)

### 相关信息：

**论文标题：An Attention-Based Deep Learning Framework for Trip Destination Prediction of Sharing Bike**

**year：2020**

**Publish :IEEE Transactions**

**Cited:35**

**Code：无**

**Data：无**

### 数据预处理：UserID 纬度 经度 时间戳

### 核心IDEA：

### 精读部分：模型组成

### 精读部分：参考资料与总结

# 杂七杂八

## 北邮超算使用指南

环境配置：

中心使用的环境是singlarty

pytorch实例:

nvidia开源了一个超算平台

镜像分享与管理

查看他们的所有镜像

任务模板

谨慎使用

https://henryf.notion.site/Pytorch-1611efdd13c84792a5dfa299c9e9631c



singalarity

 不会使用

人使用体验很差！

12月

优先级排序，申请合理的空间， 靠自觉2333

计算机专业用超算比较少





新建账户



conda





## 爬虫学习：爬取POI ：看research2022

![image-20220428122852193](https://s2.loli.net/2022/07/05/BGEOdFDelujLzJo.png)

## 爬虫笔记|POI爬取|BingMapblog

POI基本类型

[POI Entity Types - Bing Maps | Microsoft Docs](https://docs.microsoft.com/en-us/bingmaps/spatial-data-services/public-data-sources/poi-entity-types)

[Get Data Source Information - Bing Maps | Microsoft Docs](https://docs.microsoft.com/en-us/bingmaps/spatial-data-services/data-source-management-api/get-data-source-information)

[Account details - Bing Maps Dev Center (bingmapsportal.com)](https://www.bingmapsportal.com/Account)

https://docs.microsoft.com/en-us/bingmaps/spatial-data-services/public-data-sources/pointsofinterest

string DataSourceID = "20181f26d9e94c81acdf9496133d4f23";

我的accountid

```bash
1960411
```

我的key

```bash
AnCG7cHEP8TN6ZilEXG30miEDjCbt2vjWr4uJ0CuBcFD2TDLwBix6j78Lq8FMQiv
```



[Get Data Source Information - Bing Maps | Microsoft Docs](https://docs.microsoft.com/en-us/bingmaps/spatial-data-services/data-source-management-api/get-data-source-information)

获得datasource ID 的方式

**Example**: $format=json

```bash
http://spatial.virtualearth.net/REST/v1/data?$format=formatQueryOption&key=anyKeyFromTheBingMapsAccount

http://spatial.virtualearth.net/REST/v1/data?$format=json&key=AnCG7cHEP8TN6ZilEXG30miEDjCbt2vjWr4uJ0CuBcFD2TDLwBix6j78Lq8FMQiv
```

![image-20220414204323416](https://s2.loli.net/2022/07/05/8H7MX2OoKtPvkIp.png)

```bash
http://spatial.virtualearth.net/REST/v1/data?$format=atom&key=AnCG7cHEP8TN6ZilEXG30miEDjCbt2vjWr4uJ0CuBcFD2TDLwBix6j78Lq8FMQiv
```

![image-20220414204432260](https://s2.loli.net/2022/07/05/jwPoeSOpuWsQiGm.png)

atom="http://www.w3.org/2005/Atom" xmlns:bsi="http://schemas.microsoft.com/bing/spatial/2010/11/odata"

![image-20220414205748922](https://s2.loli.net/2022/07/06/jdomDHrqh6KbfSz.png)



https://docs.microsoft.com/en-us/bingmaps/spatial-data-services/public-data-sources/pointsofinterest

$符号后面的含义

https://docs.microsoft.com/en-us/bingmaps/spatial-data-services/query-api/query-options

#### 获得poi的方式





| Entity Type Name                                             | Entity Type ID |
| ------------------------------------------------------------ | -------------- |
| Agricultural Structure                                       | 6              |
| Airport                                                      | 4581           |
| Airport Runway                                               | 8              |
| Airport Terminal                                             | 237            |
| Amusement Park                                               | 7996           |
| Apparel Store (Clothing Store)                               | 9537           |
| ATM                                                          | 3578           |
| Auto Dealership                                              | 5511           |
| Auto Service & Maintenance                                   | 7538           |
| Bank                                                         | 6000           |
| Bookstore                                                    | 9995           |
| Border Post (Border Crossing)                                | 9999           |
| Bowling Alley/Centre                                         | 7933           |
| Bridge                                                       | 19             |
| Bus Station                                                  | 4170           |
| Business Facility (Administrative/Office Building, Business Center and Factory) | 5000           |
| Camp (Campground)                                            | 9517           |
| Casino                                                       | 7985           |
| Cemetery                                                     | 9591           |
| Cinema                                                       | 7832           |
| City Hall                                                    | 9121           |
| Coffee Shop                                                  | 9996           |
| Community Center (Civic/Community Centre)                    | 7994           |
| Consumer Electronics Store                                   | 9987           |
| Convenience Store                                            | 9535           |
| Convention Center (Convention/Exhibition Centre)             | 7990           |
| Court House                                                  | 9211           |
| Currency Exchange                                            | 220            |
| Dam                                                          | 45             |
| Department Store                                             | 9545           |
| Educational Structure                                        | 54             |
| Embassy                                                      | 9993           |
| Fast Food                                                    | 275            |
| Ferry Terminal                                               | 4482           |
| Financial Structure                                          | 193            |
| Fire Station                                                 | 270            |
| Fish Hatchery                                                | 59             |
| Gas Station (Petrol/Gasoline Station)                        | 5540           |
| Golf Course                                                  | 7992           |
| Government Structure (Government Office)                     | 9525           |
| Grocery Store                                                | 5400           |
| Heliport                                                     | 73             |
| Higher Education Facility (Higher Education)                 | 8200           |
| Historical Monument (Battlefield, Fort and Historical Site)  | 5999           |
| Home Improvement (Hardware and Home Furnishing Store)        | 9986           |
| Hospital                                                     | 8060           |
| Hotel                                                        | 7011           |
| Ice Skating Rink                                             | 7998           |
| Industrial Zone                                              | 9991           |
| Information Center (Tourist Information)                     | 7389           |
| Junction                                                     | 87             |
| Library                                                      | 8231           |
| Lighthouse                                                   | 94             |
| Marina                                                       | 4493           |
| Medical Service (Doctor Office and Medical Structure)        | 9583           |
| Military Base                                                | 9715           |
| Motorcycle Dealership                                        | 5571           |
| Multi Modal Station                                          | 238            |
| Museum                                                       | 8410           |
| Neighborhood (Hamlet)                                        | 9998           |
| Nightlife (Bar, Discotheque, Jazz Club, Karaoke Club and Private Club) | 5813           |
| Observation Point                                            | 114            |
| Office Supply Store (Office Supply & Services Store)         | 9988           |
| Other Accommodation (Bed and Breakfast, Cabin, Hostel, Motel and Resort) | 7013           |
| Park (Park/Recreation Area)                                  | 7947           |
| Park & Ride                                                  | 7522           |
| Parking Garage/House                                         | 7521           |
| Performing Arts (Comedy Club and Theater)                    | 7929           |
| Personal Care Facility                                       | 303            |
| Pharmacy                                                     | 9565           |
| Place of Worship (Church, Mission, Mosque, Temple and Religious Structure) | 9992           |
| Police Station                                               | 9221           |
| Populated Place                                              | 4444           |
| Port                                                         | 280            |
| Post Office                                                  | 9530           |
| Prison                                                       | 137            |
| Railway Station                                              | 4013           |
| Railway Station Entrance                                     | 273            |
| Recreational Structure                                       | 142            |
| Rental Car Agency                                            | 7510           |
| Residential Structure (Residential Area/Building)            | 9590           |
| Rest Area                                                    | 7897           |
| Restaurant                                                   | 5800           |
| Ruin                                                         | 153            |
| School                                                       | 8211           |
| Scientific Research Base                                     | 156            |
| Shopping (Market and Shopping Center)                        | 6512           |
| Ski Area (Ski Resort)                                        | 7012           |
| Specialty Store (Hobby Store, Pet Store and Warehouse Club)  | 9567           |
| Sporting Goods Store                                         | 9568           |
| Sports Complex (Playing Field and Race Track)                | 7940           |
| Stadium (Sports Centre)                                      | 7997           |
| Store                                                        | 259            |
| Tollgate                                                     | 283            |
| Transportation Service (Metro Station, Railway and Transportation Structure) | 7999           |
| Trailhead                                                    | 236            |
| Tramway                                                      | 262            |
| Transportation Service (Metro Station, Railway and Transportation Structure) | 9593           |
| Truck Dealership                                             | 9719           |
| Truck Stop (Truck Stop/Plaza)                                | 9522           |
| Tunnel                                                       | 177            |
| Vehicle Organization Office (Automobile Club)                | 8699           |
| Veterinarian                                                 | 304            |
| Weigh Station                                                | 9710           |
| Winery                                                       | 2084           |
| Zoo (Animal Park)                                            | 9718           |

```bash
http://spatial.virtualearth.net/REST/v1/data/Microsoft/PointsOfInterest?spatialFilter=nearby(40.83274904439099,-74.3163299560546935,5)&$filter=EntityTypeID%20eq%20'6000'&$select=EntityID,DisplayName,Latitude,Longitude,__Distance&$top=3&key=anyBingMapsKey

http://spatial.virtualearth.net/REST/v1/data/Microsoft/PointsOfInterest?spatialFilter=nearby(40.83274904439099,-74.3163299560546935,5)&$filter=EntityTypeID%20eq%20'6000'&$select=EntityID,DisplayName,Latitude,Longitude,__Distance&$top=3&key=anyBingMapsKey
#成功
http://spatial.virtualearth.net/REST/v1/data/Microsoft/PointsOfInterest?spatialFilter=nearby(47.610005,-122.185992,5)&$filter=EntityTypeID%20eq%20'6000'&$select=987654321123456789,Contoso Cafe,47.610005,-122.185992,5&$top=3&key= AnCG7cHEP8TN6ZilEXG30miEDjCbt2vjWr4uJ0CuBcFD2TDLwBix6j78Lq8FMQiv
#成功
http://spatial.virtualearth.net/REST/v1/data/20181f26d9e94c81acdf9496133d4f23/FourthCoffeeSample/FourthCoffeeShops?spatialFilter=bbox(47.61247675940658,-122.3237670214032,47.68239156080077,-122.27996173131822)&$format=json&key=AnCG7cHEP8TN6ZilEXG30miEDjCbt2vjWr4uJ0CuBcFD2TDLwBix6j78Lq8FMQiv

http://spatial.virtualearth.net/REST/v1/data/Microsoft/PointsOfInterest?spatialFilter=bbox(-8.6390627,41.0133802,-8.6330627,41.0193802)&$format=json&key=AnCG7cHEP8TN6ZilEXG30miEDjCbt2vjWr4uJ0CuBcFD2TDLwBix6j78Lq8FMQiv

http://spatial.virtualearth.net/REST/v1/data/Microsoft/PointsOfInterest?spatialFilter=bbox(40.83274904439099,-74.3163299560546935,40.89274904439099,-74.2663299560546935)&$format=json&key=AnCG7cHEP8TN6ZilEXG30miEDjCbt2vjWr4uJ0CuBcFD2TDLwBix6j78Lq8FMQiv
#葡萄牙的 ok的
http://spatial.virtualearth.net/REST/v1/data/Microsoft/PointsOfInterest?spatialFilter=bbox(41.0133802,-8.6390627,41.4693802,-8.0330627)&$format=json&key=AnCG7cHEP8TN6ZilEXG30miEDjCbt2vjWr4uJ0CuBcFD2TDLwBix6j78Lq8FMQiv
#葡萄牙再试试
http://spatial.virtualearth.net/REST/v1/data/Microsoft/PointsOfInterest?spatialFilter=bbox(41.0133802,-8.6390627,41.4693802,-8.0330627)&&$format=json&key=AnCG7cHEP8TN6ZilEXG30miEDjCbt2vjWr4uJ0CuBcFD2TDLwBix6j78Lq8FMQiv
#尝试typeID

http://spatial.virtualearth.net/REST/v1/data/Microsoft/PointsOfInterest?spatialFilter=bbox(41.0133802,-8.6390627,41.4693802,-8.0330627)&$filter=EntityTypeID%20eq%20'6000'&$format=json&key=AnCG7cHEP8TN6ZilEXG30miEDjCbt2vjWr4uJ0CuBcFD2TDLwBix6j78Lq8FMQiv
#尝试最大返回数量
#bingmap
http://spatial.virtualearth.net/REST/v1/data/Microsoft/PointsOfInterest?spatialFilter=bbox(41.0133802,-8.6390627,41.4693802,-8.0330627)&$filter=EntityTypeID%20eq%20'3578'&$top=30&$inlinecount=allpages&$format=json&key=AnCG7cHEP8TN6ZilEXG30miEDjCbt2vjWr4uJ0CuBcFD2TDLwBix6j78Lq8FMQiv
#一个小区域
http://spatial.virtualearth.net/REST/v1/data/Microsoft/PointsOfInterest?spatialFilter=bbox(41.0633802,-8.6390627,41.0693802,-8.6380627)&$filter=EntityTypeID%20eq%20'3578'&$top=30&$inlinecount=allpages&$format=json&key=AnCG7cHEP8TN6ZilEXG30miEDjCbt2vjWr4uJ0CuBcFD2TDLwBix6j78Lq8FMQiv
#实际操作
#查询 ATM
http://spatial.virtualearth.net/REST/v1/data/Microsoft/PointsOfInterest?spatialFilter=bbox(41.0133802,-8.6390627,41.4693802,-8.0330627)&$filter=EntityTypeID%20eq%20'3578'&$top=3&$inlinecount=allpages&$format=json&key=AnCG7cHEP8TN6ZilEXG30miEDjCbt2vjWr4uJ0CuBcFD2TDLwBix6j78Lq8FMQiv

http://spatial.virtualearth.net/REST/v1/data/Microsoft/PointsOfInterest?spatialFilter=bbox(41.0133802,-8.6390627,41.4693802,-8.0330627)&$filter=EntityTypeID%20eq%20'6'&$top=3&$inlinecount=allpages&$format=json&key=ziu1YyE2u18ghBoVIQd0~kWxeBQC0Baa5TZ4L8FzDEg~AvXvRAO5no9FUbe-oIx-lxo03d2fNUuV90eWCG1pEWmmK3MB9V5mLSej32THZj2k




http://spatial.virtualearth.net/REST/v1/data/Microsoft/PointsOfInterest?spatialFilter=bbox(41.0133802,-8.6390627,41.4693802,-8.6330627)&$filter=EntityTypeID%20eq%20'6'&$top=3&$inlinecount=allpages&$format=json&key=ziu1YyE2u18ghBoVIQd0~kWxeBQC0Baa5TZ4L8FzDEg~AvXvRAO5no9FUbe-oIx-lxo03d2fNUuV90eWCG1pEWmmK3MB9V5mLSej32THZj2k
#卡住的
-7.8980627,41.1903802
41.1873802,-7.9010627
41.1933802,-7.8950627
http://spatial.virtualearth.net/REST/v1/data/Microsoft/PointsOfInterest?spatialFilter=bbox(41.1873802,-7.9010627,41.1933802,-7.8950627)&$filter=EntityTypeID%20eq%20'4170'&$top=3&$inlinecount=allpages&$format=json&key=ziu1YyE2u18ghBoVIQd0~kWxeBQC0Baa5TZ4L8FzDEg~AvXvRAO5no9FUbe-oIx-lxo03d2fNUuV90eWCG1pEWmmK3MB9V5mLSej32THZj2k

http://spatial.virtualearth.net/REST/v1/data/Microsoft/PointsOfInterest?spatialFilter=bbox(41.1873802,-7.9010627,41.1933802,-7.8950627)&$top=3&$inlinecount=allpages&$format=json&key=ziu1YyE2u18ghBoVIQd0~kWxeBQC0Baa5TZ4L8FzDEg~AvXvRAO5no9FUbe-oIx-lxo03d2fNUuV90eWCG1pEWmmK3MB9V5mLSej32THZj2k
http.client.IncompleteRead: IncompleteRead(190 bytes read)
```

![image-20220415201120514](https://s2.loli.net/2022/07/06/23GNJoMr7qY8CkR.png)

```python
http://spatial.virtualearth.net/REST/v1/data/Microsoft/PointsOfInterest?spatialFilter=bbox(41.0133802,-8.6390627,41.4693802,-8.0330627)&$format=json&key=AnCG7cHEP8TN6ZilEXG30miEDjCbt2vjWr4uJ0CuBcFD2TDLwBix6j78Lq8FMQiv

http://spatial.virtualearth.net/REST/v1/data/Microsoft/PointsOfInterest?
spatialFilter=bbox(-8.6390627,41.0133802,-8.6330627,41.0193802)&&$format=json&key=AnCG7cHEP8TN6ZilEXG30miEDjCbt2vjWr4uJ0CuBcFD2TDLwBix6j78Lq8FMQiv
```



![image-20220414204209533](https://s2.loli.net/2022/07/06/ksj7GKCaJU9BDX6.png)





```BASH
http://spatial.virtualearth.net/REST/v1/data/accessId/dataSourceName/entityTypeName?spatialFilter=nearby(latitude,longitude,distance)&queryoption1&queryoption2&queryoptionN&jsonp=jsonCallBackFunction&jsonso=jsonState&isStaging=isStaging&key=queryKey  
0
accessID，
1
string dataSourceName = "FourthCoffeeSample";  
        // Name of entities in the data source
 2
        string dataEntityName = "FourthCoffeeShops";  
      // Unique access ID assigned to your data source by Bing Maps  
http://spatial.virtualearth.net/REST/v1/data/20181f26d9e94c81acdf9496133d4f23/FourthCoffeeSample/FourthCoffeeShops?spatialFilter=bbox(-8.6390627,41.0133802,-8.6330627,41.0193802)&key=AnCG7cHEP8TN6ZilEXG30miEDjCbt2vjWr4uJ0CuBcFD2TDLwBix6j78Lq8FMQiv



http://spatial.virtualearth.net/REST/v1/data/20181f26d9e94c81acdf9496133d4f23/FourthCoffeeSample/FourthCoffeeShops?spatialFilter=bbox(47.61247675940658,-122.3237670214032,47.68239156080077,-122.27996173131822)&$format=json&key=AnCG7cHEP8TN6ZilEXG30miEDjCbt2vjWr4uJ0CuBcFD2TDLwBix6j78Lq8FMQiv
```


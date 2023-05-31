# TFLite模型生成

## 1.新建code space

**1.选择课程作业的库**

**2.新建文件夹**

![image-20230530225035438](https://s2.loli.net/2023/05/30/xenpmQYh5IGSE2b.png)

3.新建一个python环境

![image-20230530225255076](https://s2.loli.net/2023/05/30/Kt8e6ShLmIj9ABF.png)

4.激活虚拟环境

![image-20230530230540674](https://s2.loli.net/2023/05/30/1gFslW3pLiCS4bd.png)

5.查看版本号

![image-20230530230624614](https://s2.loli.net/2023/05/30/pgoaCNAYmc6vBPT.png)

## 2.开始下载

![image-20230530230655000](https://s2.loli.net/2023/05/30/Gla6tjiXqxTObyK.png)

![image-20230530231501832](https://s2.loli.net/2023/05/30/L1afgQwG8ovSHr5.png)

下载完成

## 3.新建代码文件

![image-20230530231922985](https://s2.loli.net/2023/05/30/DwJtSaGNZkAqcor.png)

**出现这个问题：**

![image-20230531000312356](https://s2.loli.net/2023/05/31/HWCNMRwjkrhE6iq.png)

准备试试降低版本

卸载：

![image-20230531000304070](https://s2.loli.net/2023/05/31/xniBK3SZ9DVCHwR.png)

安装：

![image-20230531092511703](https://s2.loli.net/2023/05/31/v7AU4MkBfJIguKw.png)

还是错了，最后经过同学的帮助，得知需要下载1.23.0版本的numpy才可以兼容

![issue](https://s2.loli.net/2023/05/31/qKBNgWdUS5lahAi.png)

最后需要下载这个动态库，更新sudo apt update

下载成功后运行就可以了

## 4.模型训练

### 获取数据

![image-20230531095757394](https://s2.loli.net/2023/05/31/S8aDrNt7u6kXJ5Z.png)

### 加载数据集

![image-20230531095837576](https://s2.loli.net/2023/05/31/mUDds9bOgKcCwpQ.png)

### 训练tensorflow模型

![image-20230531100320649](https://s2.loli.net/2023/05/31/S5TilmBwM7XUa8A.png)

![image-20230531100332137](https://s2.loli.net/2023/05/31/resvL1TtzX9px4l.png)

### 评估模型

![image-20230531100536733](https://s2.loli.net/2023/05/31/8liQRg2LOIWG4pu.png)

### 导出tensorflow Lite模型

![image-20230531100738796](https://s2.loli.net/2023/05/31/BvhWadAwzfmRcXj.png)

导出完成
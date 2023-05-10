# 下载初始代码

```git
git clone https://github.com/hoitab/TFLClassify.git
```

![image-20230509230256799](https://s2.loli.net/2023/05/10/OKFAPyGR6pZCbWn.png)

打开新项目，有一个警告

![image-20230510091949424](https://s2.loli.net/2023/05/10/cHyONiGLws19oCf.png)

我查了一下可能是缺少SDK，下载对应版本试试

![image-20230510092152555](https://s2.loli.net/2023/05/10/7NHq6eaCbIErkV3.png)

![image-20230510092211242](https://s2.loli.net/2023/05/10/gXbno2Ll3WSsHcv.png)

![image-20230510102654834](https://s2.loli.net/2023/05/10/9QWJ6TaplXGqvtm.png)

解决：

![image-20230510103322228](https://s2.loli.net/2023/05/10/tjLrK31cQwFBs4k.png)

ok,解决了一系列好多问题。。。。。终于。。。。。运行成功了

<img src="https://s2.loli.net/2023/05/10/xKBJiF3sRlALGTt.png" alt="image-20230510103434090" style="zoom:25%;" />

# 向应用中添加TensorFlow Lite

![image-20230510103850213](https://s2.loli.net/2023/05/10/GaOslJHr5BUnYPT.png)

![image-20230510104005036](https://s2.loli.net/2023/05/10/rW2nuAPUxEClfGy.png)

![image-20230510104321480](https://s2.loli.net/2023/05/10/Wcehm4ZrsE9Pb3q.png)

# 添加代码重新运行APP

1. 定位“start”模块**MainActivity.kt**文件的TODO 1，添加初始化训练模型的代码

![image-20230510104704022](https://s2.loli.net/2023/05/10/fKTpDohFwJLNiUg.png)

2. 在CameraX的analyze方法内部，需要将摄像头的输入`ImageProxy`转化为`Bitmap`对象，并进一步转化为`TensorImage` 对象

![image-20230510104800522](https://s2.loli.net/2023/05/10/4yn2o1GVWqwcumz.png)

3. 对图像进行处理并生成结果，主要包含下述操作：

- 按照属性`score`对识别结果按照概率从高到低排序
- 列出最高k种可能的结果，k的结果由常量`MAX_RESULT_DISPLAY`定义

![image-20230510104913598](https://s2.loli.net/2023/05/10/R2srqY61uMATNwi.png)

4. 将识别的结果加入数据对象`Recognition` 中，包含`label`和`score`两个元素。后续将用于`RecyclerView`的数据显示

![image-20230510104957137](https://s2.loli.net/2023/05/10/LbBr2fyWnjz8ct7.png)

5. 将原先用于虚拟显示识别结果的代码注释掉或者删除

![image-20230510105729900](https://s2.loli.net/2023/05/10/IaNjYd1MykH4w9t.png)

运行结果：

<img src="https://s2.loli.net/2023/05/10/jTkuO2VgeH5MYcF.png" alt="image-20230510105739412" style="zoom:25%;" />
# 构建CameraX应用

## 创建项目

![image-20230426110933567](./../img/image-20230426110933567.png)

![image-20230426111359588](./../img/image-20230426111359588.png)

**换源**

```xml
pluginManagement {
    repositories {
        gradlePluginPortal()
        google()
        mavenCentral()
        maven { url 'https://maven.aliyun.com/nexus/content/groups/public/' }
        maven { url 'https://maven.aliyun.com/nexus/content/repositories/jcenter' }
        maven { url 'https://maven.aliyun.com/nexus/content/repositories/google' }
        maven { url 'https://maven.aliyun.com/nexus/content/repositories/gradle-plugin' }
        maven { url "https://jitpack.io" }
    }
}
dependencyResolutionManagement {
    repositoriesMode.set(RepositoriesMode.FAIL_ON_PROJECT_REPOS)
    repositories {
        google()
        mavenCentral()
        maven { url 'https://maven.aliyun.com/nexus/content/groups/public/' }
        maven { url 'https://maven.aliyun.com/nexus/content/repositories/jcenter' }
        maven { url 'https://maven.aliyun.com/nexus/content/repositories/google' }
        maven { url 'https://maven.aliyun.com/nexus/content/repositories/gradle-plugin' }
        maven { url "https://jitpack.io" }
    }
}
rootProject.name = "CameraXApp"
include ':app'
```

## 添加依赖

![image-20230426111944662](./../img/image-20230426111944662.png)

设置项目：![image-20230426112532600](./../img/image-20230426112532600.png)

## 创建项目布局

![image-20230426112640689](./../img/image-20230426112640689.png)

![image-20230426112700538](./../img/image-20230426112700538.png)

## 编写MainActivity.kt代码

![image-20230426113021381](./../img/image-20230426113021381.png)

## 请求必要权限

![image-20230426112958268](./../img/image-20230426112958268.png)

![image-20230426113309152](./../img/image-20230426113309152.png)

## 实现Preview用例

![image-20230426113333578](./../img/image-20230426113333578.png)

## 实现ImageCapture用例（拍照功能）

![image-20230426113559363](./../img/image-20230426113559363.png)

## 实现ImageAnalysis用例

![image-20230426113730845](./../img/image-20230426113730845.png)

![image-20230426114203146](./../img/image-20230426114203146.png)

## 实现VideoCapture用例（拍摄视频）

![image-20230426114329314](./../img/image-20230426114329314.png)

![image-20230426114412999](./../img/image-20230426114412999.png)

![image-20230426114448760](./../img/image-20230426114448760.png)

运行：

![image-20230426114911201](./../img/image-20230426114911201.png)

![image-20230426114951705](./../img/image-20230426114951705.png)

![image-20230426115032990](./../img/image-20230426115032990.png)

在虚拟机拍照一直会出现这个问题，所以寻求老师帮助，转到实体机测试，用我的手机应用会闪退，平板可以运行

![image-20230507223806478](https://s2.loli.net/2023/05/07/A4TbYO72pQseCuR.png)

运行结果：

![1683470060857](https://s2.loli.net/2023/05/07/Zc4o8uvPi29EWby.jpg)

![1683470098842](https://s2.loli.net/2023/05/07/xWegrUNRdbjzACH.jpg)

可以看到运行成功
# 创建第一个Kotlin应用程序

- 创建Basic Activity框架

![image-20230419084911416](./../img/image-20230419084911416.png)

- 等待下载
- 换源

```
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
rootProject.name = "My Application"
include ':app'
```

![image-20230419105830227](./../img/image-20230419105830227.png)

- 构建好后运行

- 这里我发现所有文件名是红色

  - 解决办法

    将.idea文件里面修改一下

  ![image-20230419131312639](./../img/image-20230419131312639.png)

![image-20230419131332676](./../img/image-20230419131332676.png)

- 运行结果

![image-20230419131600687](./../img/image-20230419131600687.png)

# 查看布局编辑器

# 布局文件

![image-20230419131945351](./../img/image-20230419131945351.png)

- 修改文本

![image-20230419132139514](./../img/image-20230419132139514.png)

- 转到申明

![image-20230419132555407](./../img/image-20230419132555407.png)

![image-20230419134147703](./../img/image-20230419134147703.png)

- 修改字体属性

![image-20230419134123497](./../img/image-20230419134123497.png)

![image-20230419135442174](./../img/image-20230419135442174.png)

- 重新运行

![image-20230419135625051](./../img/image-20230419135625051.png)

# 添加按钮和约束

- 修改布局

将id也修改

![image-20230419140651906](./../img/image-20230419140651906.png)

- 删除约束

![image-20230419141038558](./../img/image-20230419141038558.png)

- 更改组件文本

![image-20230419141523776](./../img/image-20230419141523776.png)

![image-20230419141600892](./../img/image-20230419141600892.png)

![image-20230419141631520](./../img/image-20230419141631520.png)

- 更新Next按钮

![image-20230419141800199](./../img/image-20230419141800199.png)

![image-20230419143005491](./../img/image-20230419143005491.png)

![image-20230419143144704](./../img/image-20230419143144704.png)

- 添加第三个按钮

![image-20230419143547401](./../img/image-20230419143547401.png)

![image-20230419143602138](./../img/image-20230419143602138.png)

![image-20230419144059457](./../img/image-20230419144059457.png)

修改文本

![image-20230419144609469](./../img/image-20230419144609469.png)

![image-20230419144616637](./../img/image-20230419144616637.png)

对之前的修改了一点

- 重新运行

![image-20230419150334722](./../img/image-20230419150334722.png)

报错了，查找源码应该是按钮修改了，重新引用

看代码这个按钮估计是进行重定向页面的，但是我还不知道那个按钮等会是用来跳转页面的，所以先随便指定一个

![image-20230419150517204](./../img/image-20230419150517204.png)

![image-20230419151005140](./../img/image-20230419151005140.png)

# 更新按钮和文本框的外观

![image-20230419151036389](./../img/image-20230419151036389.png)

![image-20230419151737360](./../img/image-20230419151737360.png)

![image-20230419151812929](./../img/image-20230419151812929.png)

![image-20230419151852015](./../img/image-20230419151852015.png)

![image-20230419152033456](./../img/image-20230419152033456.png)

- 设置代码自动补全

![image-20230419152137732](./../img/image-20230419152137732.png)



为Toast按钮添加一个toast消息

![image-20230419152425089](./../img/image-20230419152425089.png)

![image-20230419152841884](./../img/image-20230419152841884.png)

完善第二界面的代码

![image-20230419153309455](./../img/image-20230419153309455.png)

![image-20230419155103457](./../img/image-20230419155103457.png)

- 检查导航图

![image-20230419160142417](./../img/image-20230419160142417.png)

# 启用SafeArgs

![image-20230419160326091](./../img/image-20230419160326091.png)

![image-20230419162422232](./../img/image-20230419162422232.png)

![image-20230419162511691](./../img/image-20230419162511691.png)

# 创建导航动作的参数

![image-20230419162637065](./../img/image-20230419162637065.png)

![image-20230419162935848](./../img/image-20230419162935848.png)

![image-20230419164556615](./../img/image-20230419164556615.png)

![image-20230419164536460](./../img/image-20230419164536460.png)

- 运行结果

![image-20230419164621383](./../img/image-20230419164621383.png)

![image-20230419164632623](./../img/image-20230419164632623.png)
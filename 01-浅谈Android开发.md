# 01-浅谈Android开发

欢迎来到椰子FM,我是非著名程序员yh,做iOS应用开发.但是不务正业,有几个月没做iOS应用了
下面是我的电台的另一个主播mc,做Android应用开发

> 由于各种原因,我们电台的博客:yezifm.ga没有更新文章,只写了一个标题.但是我们会挽救这个博客的,
> 这个简书可能是我们很长时间主要更新的平台.我们也会把文章推送到微博上去.写这篇文章的时候我们
> 已经调整过几次方向了,确定下来了几个{原生Android应用开发学习分享;MIT的公开课学习分享;.NET
> 平台C#开发各种应用学习分享(包括之前Android和iOS,会用Xamarin这个技术做出来)}
> 好了,废话不多说.接下来就是我们播客内容延伸和错误修改.

第一期我们初步聊了一下Android应用开发的体验,但是我有很多年没有接触Android开发,最后一次开发

Android还是Android4.1的时候,经历过Android5.0、6.0.7.0这几个重大版本更新,都没有在接触.确实

需要学习和更新自己的知识体系,我同事也是最近接触Android应用开发的.需要加深自己的学习深度.我们

一拍即合就决定做一档节目分享自己的学习.既可以监督自己,也可以作为初学者入门的参考资料.如果Android

应用开发的大神偶然看到我们的错误.可以指出,我们虚心接受.不会死不承认的,但是播客+博客+微博的平台和

节目的形式就不改变了.因为我们是程序员出身,不是那么会说话.**不喜欢我们声音和形式也可以提建议.但是我们

坚决不改.希望大家体谅**

## 回顾CES 2017我们感兴趣的产品

- 松下GH5旗舰机无反相机:6K照片+4K连拍+4K视频
- 乐视 & 法拉第未来FF91:百公里加速,全自动泊车
- 日产BladeGlider电动超跑:空气动力学线条 + 剪刀式车门设计,再配合1+2的座椅布局
- 丰田concept-I自动驾驶汽车:采用人工智能AI助手"Yui"驱动,搭配第二代抬头显示器
- 宝马i Inside Future:前卫的HoloActive触控技术,搭配触控屏
- 黑莓 Mercury:复古情怀全键盘智能手机,黑莓自家设计的最后一款产品
- 华硕ZenFone AR:全球首款8G RAM运行内存手机,配置骁龙821,还有最近比较火热的AR(增强现实)技术
- 雷蛇 Project Valerie:全球首款三联屏笔记本电脑产品(i7+GTX1080)
- LG OLED TV W 电视:分体式设计+2.57mm的后盾,结合杜比全景声(Dolby Atmos)
- 三星Family Hub 2.0冰箱:采用21.5英寸高清触摸屏,在食品管理方面更进一步提升
- 三星FlexWash+FlexDry四合一洗衣系统:曾经4台洗衣机才能办到的事情,现在只需它一台就够了


> 从开发工具、开发模式、设计模式、第三方服务的使用、常用插件、常用框架

## Android 5.0之前的开发体验

### 开发工具

- JDK安装和配置

    - 下载最新版本的JDK

    - 配置JDK的环境变量

    - 测试是否配置正确

- Eclipse和ADT插件的安装配置,Google打包的Eclipse和ADT的开发工具

    - 下载Eclipse和ADT插件或者下载Google打包好的工具
    - 运行Eclipse和设置工作空间
    - 新建一个HelloAndroid项目
    - 新建一个Android模拟器
    - 运行HelloAndroid项目

### 开发模式

### 设计模式


MVC模式：

- View:布局的XML文件
- Controller:Activity、Fragment、Dialog等
- Model:相关的业务操作处理数据(如对数据库的操作、对网络等的操作都应该在Model层里)

### 第三方服务的使用

### 常用插件

### 常用框架

## Android 5.0之后的开发体验

### 开发工具

- JDK安装和配置

    - 下载最新版本的JDK

    - 配置JDK的环境变量

    - 测试是否配置正确

- Android Studio和SDK Tools的安装和配置

> 错误1:不能创建新项目,Gradle问题.(Android Studio 2.3)
> 解决办法:下载Gradle-3.3-all.zip放到对应的文件

> 错误2:在不联网的情况下,不能jcenter中下载必要的库
> 解决办法:连接互联网,不用科学上网

   - 下载最新版本的Android Studio
   - 下载Android各个版本的SDK
   - 新建一个HelloAndroid项目
   - 新建一个Android模拟器
   - 运行HelloAndroid项目

### 开发模式

### 设计模式

MVP模式:

- View:Activity、Fragment、Dialog、Adapter等,该层不包含任何业务逻辑
- Presenter:中介,View和Model不发生联系,都通过Presenter传递
- Model:相关的业务操作处理数据(如对数据库的操作、对网络等的操作都应该在Model层里)

### 第三方服务的使用

- 数据统计:友盟统计、百度统计
- 崩溃收集:腾讯Bugly、Bugtags
- 云存储:七牛
- 即时通信:环信、融云、阿里百川
- 推送:小米推送、腾讯推送、百度推送
- 安全加固:360加固宝、爱加密

### 常用插件

- GsonFormat:

快速将JSON字符串换成一个Java Bean,免去我们根据JSON字符串手写对应Java Bean的过程

使用方法:快捷键Alt+S;也可以用Alt+Insert选择GsonFormat

- Android ButterKnife Zelezny

配合ButterKnife实现注解,从此不用写findViewById,在Activity,Fragment,Adapter中选中布局XML的资源id自动

生成butterknife注解

使用方法:Ctrl+Shift+B

- Android Code Generator

根据布局文件快速生成对应的Activity,Fragment,Adapter,Menu

- Android Parcelable code Generator

JavaBean序列化,快速实现Parcelable接口

- Android Methods Count

显示依赖库中得方法数

- Lifecycle Sorter

可以根据Activity或者fragment的生命周期对其生命周期方法位置进行先后排序,快捷键:Ctrl+Alt+K

- CodeGlance

在右边可以预览代码,实现快速定位

- findBugs-IDEA

查找bug的插件,Android Studio也提供了代码审查的功能(Analyze-Inspect Code...)

- ADB WIFI

使用WiFi无限调试你的app,无需root权限

- AndroidPixelDimenGenerator

Android Studio自动生成dimen.xml文件插件

- JsonOnlineViewer

在Android Studio中请求、调试接口

- Android Styler

根据xml自动生成style代码的插件

- Android Drawable Importer

这是一个非常强大的图片导入插件.它导入Android图标与Material图标的Drawable,

批量导入Drawable,多源导入Drawable(即导入某张图片各种dpi对应的图片)

- SelectorChapek for Android

通过资源文件命名自动生成Selector文件

- GenerateSerialVersionUID

实现Serializable序列化bean

- Genymotion

速度较快的Android模拟器

- LeakCanary

帮助你在开发阶段方便的检测出内存泄漏的问题

- Android Postfix Completion

可根据后缀快速完成代码,这个属于拓展吧,系统已经有这些功能,如sout、notnull等

- Android Holo Colors Generator

通过自定义Holo主题颜色生成对应的Drawable和布局文件

- dagger-intellij-plugin

dagger可视化辅助工具

- GradleDependencies HelperPlugin

Maven Gradle依赖支持自动补全

- RemoveButterKnife

ButterKnife这个第三方库每次更新之后,绑定View的注释都会改变,从Bind到Inject,再到Bindview

- AndroidProguardPlugin

一键生成项目混淆代码插件

- OTTO=intellij-plugin

OTTO事件导航工具

- EventBus=intellij-plugin

EventBus导航插件

> 对于最新的EventBus3.0.0无效,替换eventbus3-intellij=plugin

- idea-markdown

markdown插件

- Sexy Editor

设置Android Studio代码编辑区的背景图

- folding-plugin

布局文件分组的插件

- Android-DPI-Calculator

DPI计算插件

- Gradle-retrolambda

在java 6 7中使用Lambda表达式插件,修改编译的jdk为java8

- Android Studio Prettify

可以将代码中的字符串写在string.xml文件中选中字符串鼠标右键选择

还可以自动书写findViewById

- Material Theme UI

添加Material主题到你的Android Studio

- .ignore

Git中想要过滤掉一些不想提交的文件,可以把相应的文件添加到.gitignore中,

而.gitignore这个Android Studio插件根据不同的语言来选择模板,就不用自己

在费事添加一些文件了,而且还有自动补全功能,过滤文件再也不要复制文件名了.我们

做项目的时候,并不是所有文件都是要提交的,比如构建的build文件夹,本地配置文件,

每个Module生成的iml文件,但是我们每次add,commit都会不小心把它们添加上去,而

gitignore就是解决这个痛点的,如果你不想提交的文件,就可以不创建项目的时候将这个

文件中添加即可,将一些通用的东西屏蔽掉

- CheckStyle-IDEA

CheckStyle-IDEA是一个检查代码风格从插件,比如像命名约定,Javadoc,类设计等方面

进行代码规范和风格的检查,你们可以遵从像Google Oracle的Java代码指南,当然也可以

按照自己的规则来设置配置文件,从而有效约束你自己更好地遵循代码编写规范

- Markdown Navigator

Markdown插件

- ECTranslation

Android Studio Plugin,Translate English to Chinese. Android Studio翻译插件

可以将英文翻译为中文

- PermissionsDispatcher plugin

自动生成6.0权限的代码

- WakaTime

记录你在IDE上工作时间

- AndroidWiFiADB

无线调试应用

- AndroidLocalizatione

可用于将项目中的string资源自动翻译为其他语言的Android Studio/Intellij IDEA插件

- TranslationPlugin

又一翻译插件,可中英互译

- SingletonTest

快速生成单例模式的预设

- BorePlugin

Android Studio自动生成布局代码插件

- jimu Mirror

能够实时预览Android布局,它会监听布局文件的改动,如果有代码变化,就会立即刷新UI

- jRebel For Android

不仅能够做到UI布局的实时预览,它甚至做到了让你更改java代码后就能实时替换apk中

的类文件,达到应用实时刷新

- sdk-manager-plugin

SDK管理插件,自动检测更新并下载

- Codata

搜索最好的Android代码

- LayoutFormatter

drakeet开发一个一键格式化你的XML文件的Android Studio插件,至于为什么不用Android

Studio自带的格式化功能而用这个插件

- Android-strings-search-plugin

一个可以通过输入文字找到strings.xml资源的插件

- ideaVim

Vim本身就是一款很优秀的文本编辑器,而Android Studio更是一款编写App应用的神器,如果两个

款优秀的软件结合在一起感觉会怎样呢?

- eventbus3-intellij-plugin

引导EventBus的post和event,主要对新版EventBus3.0.0

- Exynap

Exynap一个帮助开发者自动生成样板代码的Android Studio插件

- gradle-cleaner-intellij-plugin

> 等待解释

- MVPHelper

一款Intellj IDEA和Android Studio的插件,可以为MVP生成接口以及实现类

- Matchmarker

这是一款专为微信小程序开发的插件,目前可在Intellij IDEA中使用.它可以

帮你完成重复机械无趣麻烦的绑定方法的过程,自动的将需要新建的方法注入到

js文件中去.

- Emoji Support Plugin

让IntelliJ支持Emoji输入提醒

- Open-Uploader

上传apk文件到指定的地址,提供自定义参数

- MultiTypeTemplates

生成MultiType和itemviewprovider

- Android-ButterKnife-Plugin-Plus

Android Studio的插件,方便快速实现ButterKnife注解框架

- ApkMultiChannelPlugin

这是一个为了方便Android多渠道打包的Android Studio/IDEA插件

- CodeMaker

一个IDEA的代码生成插件,通过Velocity支持自定义代码模板来生成

代码

- adb-idea

可以一键清理缓存并重启app

- JVM Debugger Memory View

Android Studio和IDEA中一个很有用的内存调试插件

- TinyPic

压缩图片资源

- ReciteWords

一个Android Studio翻译与陌生单词记录

- TemplateBuilder

TemplateBuilder是一款能够帮助我们快速生成Android Studio Template的Android Studio插件,

将通过逐个文件去配置模板的方式改进为通过插件来实现,对于简单的模板制作,只需一键即可生成2


- Markdown Support

Markdown 支持Markdown文本

- Visual Studio Team Service

Visual Studio Team Service的代码后端处理和服务(Ops)

### 常用框架

- 网络访问框架:OKHTTP、Retrofit、Android-Async=HTTP、Volley
- 图片加载框架:Android-Universal-Image-Loader、Glide、Fresco、Picasso
- 缓存框架:DiskLruCache、Robospice
- JSON解析框架:Gson、Fastjson、Jackson
- 事件总线:EventBus、Otto
- ORM框架:GreenDAO、Litepal
- 各种开源的自定义控件、动画

> 接下来我们肯定要继续学习Android,这是我们接下来要看的Android书籍和文档

> 书籍:

> 1.第一行代码 Android 第一版 

> 2.第一行代码 Android 第二版

> 3.CommonsWare.The.Busy.Coders.Guide.to.Android.Development.Version.8.3

> 4.Java The Complete Reference Ninth Edition

> 5.Wrox.Java.Programming.24-Hour.Trainer.2nd.Edition

> 文档:
> 1.developer.android.com 英文网站

> 2.developer.android.google.cn 中文网站,**不记得网址,如果错误修改一下**

> 3.java api documents java api文档

> 视频:

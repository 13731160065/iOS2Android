创建新项目
===========================
好了，继续上次的话题。上次我们说到了创建项目，
打开AS，就会进入一个引导页面，我们肯定没创建过项目咯，选择“Start a new Android Studio project“即可
创建新项目。

![创建项目](https://github.com/13731160065/iOS2Android/raw/master/Images/创建项目.png)

点击创建后，会弹出项目的配置页面，分别输入项目名，报名(iOS里的bundleid)，不过安卓里的包名是不能随便变的，
这一点要注意，因为安卓的包名就真的是按.分成包的，比如com.wzz.xxx就会创建com文件夹，com下创建wzz文件夹，
wzz下创建xxx文件夹，这昂来的。注意安卓中的配置尽量都用英文，毕竟不是咱大中华的东西，对中文支持还不那么完美，
可能会出问题，比如路径工程名报名，都要用英文。

![创建项目2](https://github.com/13731160065/iOS2Android/raw/master/Images/AS2/创建项目.png)

路径这里我要说一下，如果MAC基础差点的打开路径选择框估计会一脸懵逼，当然也可能是我想多了，但说清楚总没坏处，
这里我在途中标明了什么对应什么文件夹，对MAC文件系统感兴趣的同学，也可以自行在网上学习一下。

![选择路径](https://github.com/13731160065/iOS2Android/raw/master/Images/AS2/选择路径.png)

点击next，进入下一个界面，这个是选择开发平台的，一般就是手机咯，你非要开发TV的话那我也拦不住你，那估计得抱
着电视调试了哈哈。直接next。

![选择平台](https://github.com/13731160065/iOS2Android/raw/master/Images/AS2/选择平台.png)

接下来的页面好像是创建了一些基本文件，xml布局文件什么的，简单提一下，以我目前的理解，安卓里的MVC就是，
Model对应Bean，View对应xml布局文件，Controller对应Activity。似乎是这个样子的。所以说学框架很重要
就算你java学的再熟也不知道什么mvc的对吧，一个平台一套框架，一套开发工具，学好了就OK，语言基本都差不多，
一精百通。直接next。

![AS初始化工程](https://github.com/13731160065/iOS2Android/raw/master/Images/AS2/AS初始化工程.png)

接下来是选择Activity，这里是不是似曾相识，跟xcode里选择项目模版类似，不过不知道是不是一样的功能。作为一个
已经开发过N款APP的大师，我选择“Empty Activity”。这里我居然有很多Activity模版，但我确定在另一个电脑上
我只有几个模版，可能是我之前下载过AS哪里配置的，或者是上一篇中下载SDK时不知道什么意思的选项那个给下的，不过
估计他们安卓用的也不多，就像iOS一样，永远是选择“Single View Application”，下一步。

![选择一个默认Activity](https://github.com/13731160065/iOS2Android/raw/master/Images/AS2/选择一个默认Activity.png)
![对比xcode模版](https://github.com/13731160065/iOS2Android/raw/master/Images/AS2/对比xcode模版.png)

下一步又让我输入Activity的名字Fuck，还真有够烦的，全默认，点下一步。Activity Name就是Controller名，
Layout Name就是xml布局文件名。说到这，我还是来说一下安卓里的布局文件，起初我以为Activity和Controller
一样，xml对应xib，但其实不是的，不清楚安卓里能不能在Activity中创建视图(貌似是不能的，这恐怕就不如iOS灵活)
安卓里的视图都是在xml里创建的，之后会详细讲到，然后视图有id，在Activity里用id获取到，再设置值，我也不会用
安卓xml的图形画布局，感觉安卓大部分还在靠代码码界面，这点对于动不动xib的我很不习惯，感觉安卓的图形化约束做的
还差一些，做安卓的看看xcode的xib就明白了，好用到爆炸。

![Activity名字](https://github.com/13731160065/iOS2Android/raw/master/Images/AS2/Activity名字.png)

好的，就是这个坑爹的页面，第一次创建项目他会给你下载一个东西，这个东西是从google.com下的，可想而知，不翻墙这里
就一直是这样，当时坑的我好惨，就算翻墙还是要下好久，可以参考一下这个，[AS创建项目卡住](http://www.jianshu.com/p/dc1cec5fb5bf)，然而这个考文件方法是win版的，没发现mac版的，建议不会折腾的小伙伴
还是乖乖翻墙吧，翻墙后创建项目，在这个页面等着就好了，要等好久的，我先睡了😪

![等待](https://github.com/13731160065/iOS2Android/raw/master/Images/AS2/等待.png)

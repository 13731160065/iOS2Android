先放个董香小姐姐镇一镇～
![董香](https://github.com/13731160065/iOS2Android/raw/master/Images/dx.jpg)

前言
==========================

本来打算转后台的，学了半截c++，学了半截unity，
突然发现，其实学系一门新技术，主要要学的是框架，
语言基础固然重要，但每一门都要先学语言基础的话太浪费时间，而且根本没必要。
就拿我学unity来说，unity众所周知用到C#或者javascript编写，我学unity的时候根本没学C#基础，
而是直接上手玩unity的开发工具，在玩的过程中了解到，原来这里所有的对象都继承一个叫做GameObject的类，
而有一些按钮之类的类和场景相关的类则是在UnityEngine中有定义。
这些东西和语言没任何关系，如果我从语言基础开始学起的话，学个2个月的语言基础后一样要学这些框架，
而且语言这东西本来就是枯燥的东西，不如从开始做东西开始，效果来的快些，在做东西的途中，遇到不清楚的语法问题，
也可以直接从网上查嘛，学以致用，学的更有动力一些。

扯的有点远了，总的来说就是，不要一味的去扣语法，直接学框架做东西来的更快一些，之后慢慢再补基础。

下载安装Android Studio
==========================

第一步，当然是下载AS咯，Eclipse虽然也能编写，但太过时了吧，现在做安卓的都用的AS，所以直接用AS吧，
对于我们这种新手来说应该还算友好，AS应该有更多针对与安卓的方便的东西。

首先就是下载，我是在这下载的：

[Android Studio中文社区](http://www.android-studio.org)

[Mac AS dmg 下载地址](https://dl.google.com/dl/android/studio/install/2.3.3.0/android-studio-ide-162.4069837-mac.dmg)

我们是iOS转安卓嘛，当然都是MAC电脑，其他小伙伴转安卓的话，赶紧买个MAC吧，哈哈哈哈哈哈哈哈哈。

mac下载dmg文件就行，win的小伙伴，肯定也知道怎么下载就不多说了，形象的说，还是来个图吧。

下载AS

![AS社区dmg](https://github.com/13731160065/iOS2Android/raw/master/Images/as中文社区dmg.png)

安装AS

![安装AS](https://github.com/13731160065/iOS2Android/raw/master/Images/安装as.png)

安装步骤，我也来讲清楚，安装AS要做的一个准备就是，**要翻墙**，不过安装的过程是不用翻墙的，
需要翻墙的是第一次创建项目的时候，要下载什么Gradu什么什么布拉布拉。哈哈忘了。😅

初始化Android Studio
============================

打开AS，就来一弹框，大体就是说要导入你自己对AS的设置，刚接触AS的话肯定是没什么设置的，
而且我有个习惯是，基本系统怎么给设置，我就怎么用，这样就算用没有设置的电脑我也一样习惯，看个人习惯了，
这里没有设置，我们选第三个，I do not ....

![没设置](https://github.com/13731160065/iOS2Android/raw/master/Images/初始化1.png)

点继续以后，就是Welcome，这个页面说的就是怎么怎么好，能用什么平台，我也没认真看英文，
看下边的几个图片觉得估计是这么个意思，直接next。

![欢迎](https://github.com/13731160065/iOS2Android/raw/master/Images/初始化2.png)

接下来是默认安装还是自定义安装，身为一个**开发者**我当然是选择自定义安装了，默认安装我怎么知道你偷偷给我安
装了什么😐

![默认安装](https://github.com/13731160065/iOS2Android/raw/master/Images/默认安装.png)

然后是选择风格，我这么正直的人，当然选择明亮的风格～

![选风格](https://github.com/13731160065/iOS2Android/raw/master/Images/选风格.png)

接下来是选要下载的东西，默认必须选的是Android SDK，这是当然了，600M，还有一个Android SDk Platform
不知道是什么东西，也下载下来吧，翻译说是“为不同Android平台创建应用程序的SDK组件”，Performance默认是打勾
的也不知道什么东西，反正不大，就选上吧，最后一个可以不用选，一看就知道，安卓模拟器，据说AS的安卓模拟器和xcode
的iOS模拟器天差地别，性能极差，超级难用，他们安卓都用真机调试的，而且还得占用700M内存，果断不装，后边用真机
调试就可以。这里我之前装过AS，所以下边有个警告一样的东西，他说的是，已存在ASSDk，已存在的部分她不会装，只会
帮我装缺少的部分，so，这里我应该可以省去很多下载的时间。提示一下，这里应该是不需要翻墙的，但如果遇到下载不动
的情况，也可以翻墙试试，我记得我是第一次创建工程的时候，会出现一个进度条一直呆在那，后来查了一下才知道，需要
翻墙下东西，好，点击继续。

![预装SDK](https://github.com/13731160065/iOS2Android/raw/master/Images/ASSDK.png)

接下来这一步，有点像虚拟机选内存似的，具体意思应该也就是AS最大能用多少内存，直接下一步。

![选内存](https://github.com/13731160065/iOS2Android/raw/master/Images/选内存.png)

最后就是看一眼你自己的配置，我很自信的直接点“Finish”

![初始化结束](https://github.com/13731160065/iOS2Android/raw/master/Images/初始化结束.png)

接下来AS会自动下载SDK，这里有个按钮叫“Show Detail”，点开以后会有下载的详情，你可以看到他在下载什么，以缓解
你焦急等待的心情，或者你也可以去泡杯咖啡打盘王者洗洗澡啥的。噢对了，还是不要洗澡了，期间她会找你要管理员权限的，
记得看着点。下载完成后点击“Finish”。安装完成。

![下载SDK](https://github.com/13731160065/iOS2Android/raw/master/Images/下载SDK2.png)

完成后会自动打开创建项目页面，我们肯定没创建过项目咯，选择“Start a new Android Studio project“即可
创建新项目，关于创建项目，我们下期再说，有问题记得看下期噢。

![创建项目](https://github.com/13731160065/iOS2Android/raw/master/Images/创建项目.png)


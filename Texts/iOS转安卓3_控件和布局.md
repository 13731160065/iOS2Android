控件
====================

前一期我们学习了创建一个helloworld的工程。工程中有一个label，写着helloworld，那么接下来，我们就开始进行
控件和布局的学习，控件当然有很多了，首先上一张图

![控件1.png](https://github.com/13731160065/iOS2Android/raw/master/Images/AS3/控件1.png)

图中打开了一个xml，这个xml就是布局文件，在右侧可以看到一个手机的预览样式，今天我们先学几个简单的控件

1.**TextView**，安卓中的TextView就是iOS里的UILabel。

2.**Button**，很简单，对应iOS的UIButton。

3.**EditText**，对应iOS里的TextField。

4.**View**，对应iOS里的UIView。并且同样，这些视图也都继承于View，和UIView有类似效果

我们先来讲一下`View`，`View`上有一个属性是`android:background="@color/backColor"`这个属性可以设置他的背景
颜色，顺便说一下，AS官方建议文字统一设置在`strings.xml`，颜色统一设置在左侧文件夹里的`color.xml`文件里，
颜色声明的代码是`<color name="backColor">#f0f0f0</color>`

xml代码中标有`layout`的代码都是用来布局的，等会再讲，先看一下今天这4个控件的基本属性

接下来我们要讲的是`TextView`和`EditText`，之所以放一起讲，是因为这两个东西的属性其实是差不多的，主要就是一个
`text`文字属性，设置文字的代码是这样的`android:text="xxxxxxxxx"`，当然还有`android:textAlignment="center"`文本对齐样式，这些东西大家可以自己摸索，`EditText`有一个属性叫做
`android:inputType="textPersonName"`这个是文本输入的类型，还可以设置成加密等样式的

下面我们讲一下`Button`，`Button`最重要的功能就是点击了，他有一个属性叫做`android:onClick="btnClick"`，
等号后边写的"btnClick"是点击事件的方法名，见图，关联好这个后，点击就可以触发点击事件了，是不是很简单

![按钮点击方法.png](https://github.com/13731160065/iOS2Android/raw/master/Images/AS3/按钮点击方法.png)

今天的控件就讲到这，下面我们来讲讲安卓的布局

布局
======================

布局相关方法是所有控件共有的方法，安卓中其实有很多类型的布局，不过刚开始学，学多了容易乱，也记不住那么多，我们就
不讲那么多布局，我们今天着重讲一下安卓的`相对布局`。其实这个`相对布局`很接近iOS的加约束，控件相对上下左右的距
离，这样的布局方式。

那下面我就按照iOS的约束方式讲一下安卓的布局

安卓的约束和约束的数值是分离的，可以讲参照物设置为父视图，也可以参照某个视图，比如下边第二个约束，是参照一个
button来布局的

**约束类型**

`app:layout_constraintTop_toTopOf="parent"`//添加视图上部对父视图上部的约束

`app:layout_constraintTop_toBottomOf="@+id/button"`//添加视图上部对button视图下部的约束

`app:layout_constraintLeft_toLeftOf="parent"`//添加视图左部对父视图左部的约束

`app:layout_constraintLeft_toRightOf="parent"`//添加视图左部对父视图右部的约束

`app:layout_constraintRight_toRightOf="parent"`//添加视图右部对父视图右部的约束

`app:layout_constraintRight_toLeftOf="parent"`//添加视图右部对父视图左部的约束

`app:layout_constraintBottom_toBottomOf="parent"`//添加视图下部对父视图下的约束

`app:layout_constraintBottom_toTopOf="parent"`//添加视图下部对父视图上部的约束

**约束值**

约束值

`android:layout_marginTop="8dp"`//上部距离

`android:layout_marginLeft="8dp"`//左侧距离

`android:layout_marginRight="8dp"`//右侧距离

`android:layout_marginBottom="8dp"`//底部距离

`android:layout_height="20dp"`//控件高度

`android:layout_width="0dp"`//控件宽度


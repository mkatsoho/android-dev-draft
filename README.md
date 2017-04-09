# android-dev-draft

外行安卓开发笔记


## 概述

可简可繁，可快可慢。读一下这个先。 https://www.zhihu.com/question/27069588

android的java使用的类库和后台开发用到的类库差别很大。所以有后台java开发的人，绝不等于可以很容易的上手去开发android

安卓的开发的套路不如ios，没有一个现成的1，2，3这样的步骤。所以不同人写的同一款应用，从代码角度讲可能差别很大。也可能会很烂。

## 开发工具

目前（by Mar，2017）最流行的，也是效率比较高的IDE https://developer.android.com/studio/index.html
最流行的，build／package工具是gradle


## 开发方式

- 原生开发： 基于android java类库和控件来开发 （大部分）
- 基于html5开发：例如（据说）今日头条的app，目前不多。（目前不多，但发展速度很快）
- 原始加html5: 大部分原始，里面嵌入少量的html5容器，例如小米商城（登录的一小部分是嵌入的html5）。（很多）
- html5加壳：就是一个webview容器里面访问html5网站，外面加一个java 壳做成的app，（不推荐）

## 开发过程 （针对原生开发）

先看看这个教程，TP的教程都很精炼（不过我没看过） - https://www.tutorialspoint.com/android/

这个就只作为参考吧，google的教程很完整和很冗长 - https://developer.android.com/training/index.html


了解安卓控件，特性，类库。了解一下吧，android提供的控件和框架远远不够。

开源类库 - https://github.com/Tim9Liu9/TimLiu-Android  
开源类库 - https://github.com/Trinea/android-open-project


## 开发难点

- android的事件处理
有太多的app页面切换的方式，很多时间需要加hook，处理不好（比如遗漏了）会使得状态机不完整。

- android的API／控件
需要了解各种API／控件的细节，特别是做特殊的功能，比如在app里面和在屏保的使用的控件不同。如果只是访问和展示服务端的数据，则不是问题

- webview是个双刃剑
或者使用android的UI控件，尽量避免使用webview控件（是一个类似browser的html容器）

- 如果要发布的话
如果通过推广获得用户，并发布到google play，就还要熟悉如何推广，如何提高排名，如何获得留存等统计信息。否则，可以忽略。



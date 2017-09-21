# 前言 #
---
人生苦**短**，**快**用派森！([Life is short](http://www.sebsauvage.net/python/ "BruceEckel-PythonMotto"), [U need Python](http://zoomquiet.io/ "PythonSloganCN")!)：这句Python的Slogan是[那个秀才](http://zhouguoqiang.cn/ "作者")修订的，主要突出“紧迫”和“敏捷”。

带侬装逼[带侬飞](https://xkcd.com/353/ "FlyWithPython")，带侬杵进蟒蛇堆！这个是[Bob·NX](http://www.nagexiucai.com/ "作者")根据宣传漫画转译的。

这套书主要讲解Python技术栈的基础知识，共三卷：

- 第一卷：语法、标准库和设计模式。

- 第二卷：包管理、WxPython应用开发和打包。

- 第三卷：WSGI、Web框架和Tornado。

需要强调的是，**本书面向Python初学者**！不涉及解释器和字节码、对象的内存结构、运行时垃圾回收、多任务调度原理等话题，就是“把Python当作机器的原生语言来用”。

**知识的获取是不断迭代的**，很多同样的主题会在不同的章节（甚至在以后可能出现的提高专题篇中）重复出现、内容重点却是阶梯式上升的！对于有经验的朋友，把某些章节的某个主题单独拿出来看，确实是不完善，甚至是偏颇的，因为有些事情这个时候还不宜展开讲。大家回想自己求知的路径：小学数学主要是限于自然数范畴，并不能一下子将整个数集暴露给天真的孩子。**有疑问，不用急；要么三五行以内会给出说明、要么可以暂且搁置以待后释**。

做三卷安排，主要考虑到：

- 不精通基本语法、不熟悉标准库、不了解软件工程中常用的设计模式，就不能高效地驾驭Python这门语言、就不能体会Python动态特性的精髓、就不能写出高内聚低耦合的代码；由于Python本身接近自然语言的特性，甚至让很多略懂英文而没有任何计算机编程基础的新手通过几天甚至数小时的学习，就认为已经达到可以参与到实战项目的开发中，岂不知写出的代码维护难度极大，工作过程中碰到一些基础问题就无从下手，只能借助搜索引擎、然后复制粘贴。笔者将这部分内容，融入“[HowtoPython](https://github.com/nagexiucai/howtopython "HowtoPython")”项目中。

- 不懂包管理就不能拥抱浩瀚且强大的Python第三方库、就不能收到事半功倍的效果。这部分笔者将通过实现一个可用的插件化桌面工具“[FeiYang](https://github.com/nagexiucai/feiyang "FeiYang")”来阐述，并最终打包发布到Windows平台上，进一步夯实Python基础。

- 不会用Python开发Web，一定是有志于用Python改变世界者最重要的缺憾。笔者选择时下流行的框架实现个人博客“[Vast](https://github.com/nagexiucai/vast "Vast")”，引导大家理解Web原理。

掌握好上述内容，就算是入门了。

对于Python的VersionII和VersionIII有重大区别的，会做出对照。

讲义中：

- 会根据需要**灵活转换人称、场景**，目的是尽可能清晰地表达、让读者更容易领悟
- 会给必要的参考提供链接，请读者**务必抓住主干**，不要在这些庞杂的周边信息上耗费太多时间和精力
- 会针对某些操作过程做**GIF**图片，若觉得滚动速度快，可在图片上单击转到有序JPG列表

# 排版 #
---
- **粗体**表示是重点
- *斜体*表示有内涵
- [链接](https://github.com/nagexiucai/manuscripts/blob/master/Python半深入讲义.md "本书")表示用参考
- 代码会有明确段落
- 缩进表达所属关系
- 编号不会超过十六（否则划分不规范）

各种形式，都是为了打造不同于别的Python入门教程的内容，做到：

- 深入的刚刚好
- 不只是Python基础

# 目录 #
---
## [第一卷](https://github.com/nagexiucai/manuscripts/blob/master/Python半深入讲义/第一卷.md "卷一") ##
### [自曝家事](https://github.com/nagexiucai/manuscripts/blob/master/Python半深入讲义/自曝家事 "自曝家事") ###
- [缘起](./Python半深入讲义/自曝家事/缘起.md "缘起")
- [资源](./Python半深入讲义/自曝家事/资源.md "资源")
- [展望](./Python半深入讲义/自曝家事/展望.md "展望")
### [子丑寅卯](https://github.com/nagexiucai/manuscripts/blob/master/Python半深入讲义/子丑寅卯 "子丑寅卯") ###
- [环境搭建](./Python半深入讲义/子丑寅卯/环境搭建.md "环境搭建")
- [初体验](./Python半深入讲义/子丑寅卯/初体验.md "初体验")
- [原则](./Python半深入讲义/子丑寅卯/原则.md "原则")
### [背诵默写](https://github.com/nagexiucai/manuscripts/blob/master/Python半深入讲义/背诵默写 "背诵默写") ###
- [类](./Python半深入讲义/背诵默写/类.md "类")
- [实例](./Python半深入讲义/背诵默写/实例.md "实例")
- [对象](./Python半深入讲义/背诵默写/对象.md "对象")
- [数字](./Python半深入讲义/背诵默写/数字.md "数字")
- [文本](./Python半深入讲义/背诵默写/文本.md "文本")
- [容器](./Python半深入讲义/背诵默写/容器.md "容器")
- [函数](./Python半深入讲义/背诵默写/函数.md "函数")
### 啥猫腻儿 ###
- 操作平台
- 解释系统
### 众人拾柴 ###
- 线程
- 协程
- 圣旨
### 量体裁衣 ###
- 独一无二
- 左手右手
- 吃喝拉撒
### 有趣的是 ###

## 第二卷 ##
### 恰同学少年 ###
### 形而上 ###

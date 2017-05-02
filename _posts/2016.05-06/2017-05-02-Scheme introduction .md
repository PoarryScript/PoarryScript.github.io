---
layout: post

---
layout: post
title: Scheme简介和开发工具介绍
date: 2017-05-02 21:50:00
categories: [Scheme]
tags: [Scheme]
----------

## 简介 ##
   **Scheme**是由Gerald J. Sussman 和 Guy L. Steel Jr. 在1975发明的一种编程语言(programming lanugage),[Scheme](https://zh.wikipedia.org/wiki/Scheme "Scheme")是一种函数式编程语言，是Lisp的两种方言之一。

## Introductory ##
  在Scheme得[官网](http://schemers.org/ "http://schemers.org/") 首页有个The Regular Fare ，这里面有 学习、实践、应用等一系列分类如下：
![](http://i.imgur.com/SNHiVYI.jpg)
  
- 推荐的学习书籍我列举一二 <Br/>
   [Structure and Interpretation of Computer Programs](https://mitpress.mit.edu/books/structure-and-interpretation-computer-programs "https://mitpress.mit.edu/books/structure-and-interpretation-computer-programs")<Br/>
   [The Little Schemer](http://www.ccs.neu.edu/home/matthias/BTLS/ "http://www.ccs.neu.edu/home/matthias/BTLS/")<Br/>
- 图像开发环境 <Br/>
  越来越多的软件集成Scheme 的图形化开发环境，以下软件任选其一就可。<Br/>
 [3DScheme](http://www.schemers.com/3dscm1.html "http://www.schemers.com/3dscm1.html"), [3DScheme Pro ](http://www.schemers.com/3dscm1.html)和 [EdScheme](http://www.schemers.com/edschem.html)<Br/>
[Bee](http://www-sop.inria.fr/mimosa/fp/Bigloo/)<Br/>
[DrScheme](http://www.drscheme.org/)<Br/>
[fluxus](http://www.pawfal.org/fluxus/), 是一个在线编程的环境，特别cool<Br/>
[SchemeWay](http://schemeway.sourceforge.net/) <Br/>
[Pilo Visual Tools for Scheme](http://www.davidpilo.com/pvts/)
- [SRFI](https://srfi.schemers.org/)是Scheme得一些比较实用的lib库，在这里可以采用别人的成功同时也可以回馈。
- Scheme相关的Job可查看[这里](http://schemers.org/Positions/)


## 环境 ##
 我用的软件是[fluxus](http://www.pawfal.org/fluxus/packages/)。环境配置很简单，在fluxus得软件下载地方分别有介绍配置方法，用OSX来举例 ：
 下载完安装包之后

> copy the app to /Applications! Install Jack OSX version 0.81 for Tiger for sound input。


 就可以了。
我是win环境所以只需要下载 压缩包然后拷到C:Program Files这个目录下就好了。
> C:\Program Files\Fluxus\bin
然后右键fluxus.exe以管理员身份运行就会出来
![](http://i.imgur.com/kK9yze8.png)
至此 Scheme的开发环境就算搭建成功。


是不是hin简单~
---
layout: post
title: '《Android开发艺术探索》，读书笔记（1）Android生命周期'
date: 2019-04-12
author: 邱涛
cover: 'http://on2171g4d.bkt.clouddn.com/jekyll-banner.png'
tags: Android 生命周期
---

> Activity： 前台和可见的区别，对调用生命周期方法的影响.

##  生命周期图示  ##
![Android 生命周期](assets\img\androidlifecycle.png)


##  问题  ##
1. onStart onResume、onPause onStop从描述上差不多，对我们来说有什么实质的不同？
2. 假设当前的Activity的为A，如果这是用户打开一个Activity B，那么B的onResume和A的onPause哪个先执行呢？


## 答案 ##
问题1：onStart和onStop是从Activity是否可见的角度来回调的，而onResume和onPause是从Activity是否位于前台这个角度来回调的，除了这种区别，在实际使用中没有其他区别。

问题2：A先执行，B在执行。



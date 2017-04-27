nb-mobile-slide
===========================

用于处理滑动事件

## 安装方法

```

# 全局安装
npm install nb-mobile-slide -g

# 本地安装
npm install nb-mobile-slide

# 本地安装并保存到项目的package.json文件
npm install nb-mobile-slide --save

```

## 使用方法

```

# 加载组件
var nbMobileSlide = require('nb-mobile-slide');

# 新建处理滑动对象
var slideHandler = new nbMobileSlide(selector, dir, endFun, lock, transEnd);

* selector：DOM对象或者标识DOM节点的ID字符串
* dir：表示滑动的方向，可以为H或V，H表示沿水平方向滑动，V表示沿垂直方向滑动，默认值为H
* endFun()：手指松开后的回调函数
* lock：表示是否锁定DOM节点，锁定后将阻止事件的默认行为和防止事件冒泡
* transEnd(event)：DOM对象的动画结束后的回调函数，输入参数event表示事件对象

```

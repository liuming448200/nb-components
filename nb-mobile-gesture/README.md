nb-mobile-gesture
===========================

用于处理手势事件

## 安装方法

```

# 全局安装
npm install nb-mobile-gesture -g

# 本地安装
npm install nb-mobile-gesture

# 本地安装并保存到项目的package.json文件
npm install nb-mobile-gesture --save

```

## 使用方法

```

# 加载组件
var nbMobileGesture = require('nb-mobile-gesture');

# 新建处理手势对象
var gestureHandler = new nbMobileGesture(selector, moveFun, endFun, lock, transEnd);

* selector：DOM对象或者标识DOM节点的ID字符串
* moveFun(dom, dx, dy)：手指移动过程中的回调函数，输入参数dom表示selector对应的DOM对象，dx表示沿X轴移动的位置差，dy表示沿y轴移动的位置差
* endFun(dom, dx, dy, t)：手指松开后的回调函数，输入参数dom表示selector对应的DOM对象，dx表示沿X轴移动的位置差，dy表示沿y轴移动的位置差，t表示手指移动的方向，可以为left，right，up或down
* lock：表示是否锁定DOM节点，锁定后将阻止事件的默认行为和防止事件冒泡
* transEnd(event)：DOM对象的动画结束后的回调函数，输入参数event表示事件对象

```

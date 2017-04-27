nb-mobile-click
===========================

用于处理点击事件

## 安装方法

```

# 全局安装
npm install nb-mobile-click -g

# 本地安装
npm install nb-mobile-click

# 本地安装并保存到项目的package.json文件
npm install nb-mobile-click --save

```

## 使用方法

```

# 加载组件
var nbMobileClick = require('nb-mobile-click');

# 新建处理点击对象
var clickHandler = new nbMobileClick(selector, clickFun, css);

* selector：DOM对象或者标识DOM节点的ID字符串
* clickFun：点击后的回调函数
* css：DOM节点按下时的CSS字符串

```

---
layout: post
title:  "关于父容器设置了overflow:hidden,绝对定位的元素显示情况"
date:   2016-06-16
excerpt: "今天写样式的时候，发现父容器定义了overflow:hidden;position:relative;子元素的绝对定位超出父容器的部分会被裁剪。"
tag:
- css
comments: true
---

今天写样式的时候，发现父容器定义了```overflow:hidden;position:relative;```子元素的绝对定位超出父容器的部分会被裁剪。

没有设置```position:relative;```的情况

<div style="width:200px;height:200px;overflow:hidden;border:solid 1px red;">
	我没有设置position
	<div style="position:absolute;left:300px;bottom:-100px;width:200px;height:200px;border:solid 1px blue;">我是绝对定位!父容器是红色的框框。</div>
</div>

设置```position:relative;```的情况

<div style="width:200px;height:200px;overflow:hidden;border:solid 1px red;position: relative;">
	我没有设置position
	<div style="position:absolute;left:100px;bottom:-100px;width:200px;height:200px;border:solid 1px blue;">我是绝对定位!父容器是红色的框框。</div>
</div>
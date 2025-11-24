
---
title: "CSS-day5"
date: 2025-11-24T12:00:00+08:00
draft: false
summary: "这是我第三天学习CSS。"
---

大概内容：
	层复合选择器、CSS特性、背景属性、显示模式
<br>
<hr>
<!--more-->

# （一）、选择器

	1.结构伪类选择器
		作用：根据元素的结构关系查找元素
		选择器：
			li:first-child：查找第一个li元素
			li:last-child：查找最后一个li元素
			li:nth-child：查找第N个li元素（第一个元素N值为1）
			li:nth-child（2n）：查找第偶数个li元素（第一个n值为0）
			li:nth-child（-n+5）：查找前5个li元素（第一个n值为0）
			

	2.伪元素选择器
		作用：创建虚拟元素（伪元素），放装饰性内容
		选择器：
			div::before：在div元素**里面**的最前面添加一个伪元素
			div::after：在div元素**里面**的最后面添加一个伪元素
			注意：
				必须设置conten：“”属性，用来设置伪元素的内容，没有则留空
				伪元素默认是行内显示模式
				权重和标签选择器相同
		


# （二）、PxCook软件
	PxCook（像素大厨）是一款切图设计工具软件。支持PSD文件的文字、颜色、距离自动智能识别。
	1.开发面板（自动智能识别）
	2.设计面板（手动测量尺寸和颜色）


# （三）、盒子模型
	作用：布局网页，摆放盒子和内容

	1.组成（由内向外）
		width&height：内容区域
		padding：页边距（盒子与边缘之间）
		border：边框线
		margin：外边距（盒子外面）

	2.边框线
		属性名：border（bd）-方向名词
		属性值：
			size
			solod：实线
			dashed：虚线
			dotted：点线
			color
		exp：border-bottom: 5px dashed red;
		

	3.内边距
		作用：设置内容与盒子边缘之间的距离
		属性名：padding-方向名词（上右下左--顺时针）
		exp：padding: 20px 30px 40px 50px;


	4.尺寸计算
		盒子尺寸 = 内容尺寸 + border尺寸 + 内边距尺寸
		解决方式：
			1、手动计算
			2、内减模式：box-sizeing:bordfer-box

	5.外边距
		作用：拉开两个盒子之间的距离
		属性名：margin
		用法与padding一样
		注意：外边距不会撑大盒子


# （四）、其他设置

	1.版心居中（要求盒子有宽度）
		margin: 0 auto

	2.清除默认样式（通配符标签）
		*{margin: 0 border:0}

	3.内容溢出overflow属性
		作用：控制溢出元素的内容的显示方式
		属性名：overflow
		属性值：
			hidden：溢出隐藏
			scroll：溢出滚动（无论是否溢出，都显示滚动条位置）
			auto：溢出滚动（溢出才显示滚动条位置）

	4.外边距问题-合并和塌陷
		1、合并
			场景：垂直排列的兄弟元素，上下margin会合并
			现象：取两个margin中较大值生效
		2、塌陷
			场景：父子级标签，子级添加上外边距margin-top会产生塌陷问题
			现象：导致父级一起向下移动
			解决方法：
				①取消子级margin，父级设置padding
				②父级设置overflow：hidden
				③父级设置border-top

	5.行内元素垂直内外边距
		场景：行内元素添加margin和padding，无法改变元素垂直位置
		解决方法：给行内元素加line-height可以改变垂直位置

	6.圆角
		作用：设置元素的外边框为圆角
		属性名：border-radius
		属性值：数字+px / 百分比
			注：属性值是圆角半径
		exp：border-radius: 15px 20px 25px 30px;
		常见应用：
			1、正圆形状：border-radius：50%;（最大值）
			2、胶囊形状：border-radius：[高度的一半];

	7.阴影
		作用：给元素设置阴影效果
		属性名：box-shadow
		属性值：X轴偏移量 Y轴偏移量 模糊半径 扩散半径 颜色 内外阴影
			注：X轴偏移量 Y轴偏移量必须写
				默认是外阴影，内阴影需添加inset
		exp：box-shadow: 5px 5px 10px 1px gray inset;


# （五）、综合案例
	1.产品卡片
	2.新浪新闻

请关注公众号获取更多信息！！！
![alt text](./wechat.jpg)
<img src="./wechat.jpg" alt="微信公众号：茉莉智元" width="200" height="200">
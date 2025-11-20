
---
title: "CSS-day4"
date: 2025-11-20T12:00:00+08:00
draft: false
summary: "这是我第一天学习CSS。"
---

大概内容：
	层复合选择器、CSS特性、背景属性、显示模式
<br>
<hr>
<!--more-->

# （一）、复合选择器
	定义：两个或多个基础选择器通过不同方式组合而成

	1.后代选择器
		写法：父选择器 子选择器{CSS属性}，父子之间为空格
			 <style>
			        div span {color: red;}
			</style>
	2.子代选择器
		写法：父子之间为 > 符号
			 <style>
			        div>span {color: red;}
			</style>

	3.并集选择器
		作用：选中多组标签设置相同样式
		写法：选择器1，选择器2，...，选择器N{CSS属性}，选择器之间用逗号隔开
		<!-- 并集选择器 -->
			<style>
				span, p {font-size: 20px;}
			</style>

	4.交集选择器
		作用：选择同时满足多个条件的元素
		写法：选择器1选择器2{CSS属性}，选择器之间没有符号
			<style>
			        p.box {background-color: yellow;}
			</style>

	5.伪类选择器
		作用:选中元素的某个状态设置样式（鼠标悬停时变化）
		写法：选择器：hover{CSS属性}
			   <style>
				   a:hover {color: orange;}
			   </style>
		注意：任何标签都可以这么用
		拓展：超链接的四个状态（必须按以下顺序）
				link：访问前
				visited：访问后
				hover：鼠标悬停
				active：点击时

# （二）、CSS特性
	CSS特性：化简代码/定位问题，并解决问题

	1.继承性
		子级（未定义的属性）默认继承父级的文字控制属性
	
	2.层叠性
		特点：
			相同的属性，后面的覆盖前面的
			不同的属性叠加
	
	3.优先级
		一个标签使用了多种选择器时，基于不同种类选择器的匹配规则
		规则：选中标签的范围越大，优先级越低
		公式：通配符<标签<类<id<行内样式<!important
		继承权重最低

# （三）、Emmet写法

	代码的简写方式，输入缩写
		1.div+p：同级标签
		2.div>p：父子级标签
		3.span*3：多个相同标签
		4.div{内容}：有内容的标签
		5.标签名.类名：类选择器
		6.标签名#id名：id选择器

# （四）、背景属性

	1.背景图：装饰性图片
		background-color：背景色
		background-image：背景图
		background-repeat：背景图平铺方式
		background-position：背景图位置
		background-size：背景图缩放
		background-attachment：背景图固定
		background：背景图复合属性

# （五）、显示模式
		作用：根据标签的显示模式选择合适的标签展示内容

	1.块级
		独占一行
		宽度默认是父级的100%
		添加宽高属性生效

	2.行内元素
		一行共存多个
		尺寸由内容撑开

	3.行内块元素
		一行共存多个
		默认尺寸由内容撑开
		加宽高生效

	4.转换显示模型
		属性名：display
		属性值：block、line-block

# （六）、综合案例
	热词、banner效果
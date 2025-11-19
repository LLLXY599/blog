---
title: "CSS-day3"
date: 2025-11-19T12:00:00+08:00
# 这一行必须是 false，并且不能有引号！
draft: false
summary: "这是我第一天学习CSS。"
---

大概内容：
    层叠样式表CSS的引入方式、选择器、调节工具等
<br>
<hr>
<!--more-->
# （一）、层叠样式表-初体验（美化HTML）
	html文件中加选择器，例如
		<head>
			<title></title>
			<style>
			        p {
			            color: blue;
			            font-size: 20px;
			            font-weight: bold;
			        }
			</style>
		</head>
		<body>
			<p>CSS体验</p>
		</body>

# （二）、引入方式

## 内部样式：学习使用（如上）

## 外部样式表：开发使用
	1.写在单独的css文件.css中
		p {
			color: blue;
			font-size: 20px;
			font-weight: bold;
		}
	2.html文件中写link
		<title></title>
		<link rel="stylesheet" href="./04-css1.css">

## 行内样式：配合JavaScript使用
	css卸载标签的style属性值中
	    <q style="color: rgb(0, 38, 255);">体验css 引用</q>

# （三）、选择器
	作用：查找标签，设置样式

## 基础选择器

	1.标签选择器
		使用标签名作为选择器
		特点：设置同名标签，显示相同样式

	2.类选择器
		作用：差异化设置标签的显示效果
		步骤：
			1.定义类选择器-》.类名
				.highlight-new {
			            background-color: yellow;
				}
				.special {
			            color: green;
			            font-size: 18px;
			        }
			2.使用选择器-》标签添加 class=“类名”
				<div class="highlight-new">2.类选择器</p>
				<p class="highlight-new special">类选择器</p>
		特点：
			1.一个类选择器可以给多个标签使用
			2.一个标签可以使用多个类名

	3.id选择器
		作用：同类选择器
		场景：配合JS使用
		步骤：
			1.定义id选择器-》#id名
			2.使用id选择器-》标签添加 id=“id名”
		规则：同一个id名在一个页面只能用一次

	4.通配符选择器
		作用：无序调用，查找页面所有标签，设置相同样式，开发初期默认样式
		格式：*

## 画盒子
	目标：使用合适的选择器画盒子
	属性：width，height，background

## 文字控制属性
	文字大小：font-size
	字体粗细：font-weight
	字体倾斜：font-style
	行高：line-height
	字体族：font-family
	字体复合属性：font
	文本缩进：text-indent
	文本对齐：text-align
	修饰线：text-decoration
	颜色：color

## 调试工具-google浏览器
	作用：检查、调试代码
	1.错误有黄色叹号
	2.css前面有多选框，勾选则生效，未勾选则不生效

## 综合案例--新闻详情

请关注公众号获取更多信息！！！
![alt text](../../../assets/img/wechat.jpg)
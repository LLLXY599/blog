---
title: "HTML-day1"
date: 2025-11-17T12:00:00+08:00
# 这一行必须是 false，并且不能有引号！
draft: false 
description: "这是我第一天学习HTML。"
---

大概内容：
	准备开发环境、标签语法、综合案例


<!--more-->
（一）、准备开发环境
	①vscode（编写代码）+Google浏览器（看效果）
	②插件：open in browser(打开网页)
	③把Google浏览器设置为默认浏览器

（二）、标签语法
	定义：超文本（链接）标记（标签<>）语言
	注：用（）代替<>



（三）、基本骨架
	①快速生成骨架：！
	②网页名字：title
	③整个网页：html
	④网页头部：head
	⑤网页主体：body

（四）、标签关系
	①父子关系（嵌套关系）
	②兄弟关系（并列关系）

（五）、文字标签
	ctrl + / ：注释捷键
	标题标签：h1至h6（双标签），独占一行，逐渐减小字体
		注：h1在一个网页中只用一次，其他的没有次数限制
	(strong)文字(/srong)：加粗
	b：加粗
		注：vscode中手动换行没用
	br：换行
	hr：水平线
	em / i：倾斜
	ins / u：下划线
	del / s：删除线

（六）、图像标签及属性
	(img src="图片的url")
	alt：替换文本，图片无法显示的时候显示的文字
	title：鼠标悬停在图片上的时候显示的文字
	width：宽度
	height：高度

（七）、超链接标签及属性
	（a  href=" 链接")文字（/a)
	href：写#代表空链接
	target：打开新窗口跳转

(八)、音频标签及属性
	(audio src=" url ")(/audio)
	cotrols：显示音频控制面板，属性名与属性值一样简写
	loop：循环播放
	autoplay：自动播放，禁用

（九）视频标签及属性
	(video src=" url ")(/video)
	cotrols：显示音频控制面板，属性名与属性值一样简写
	loop：循环播放
	autoplay：自动播放，禁用
	muted：静音播放

（十）、综合案例-个人简介
	思路：从上到下，先整体再局部


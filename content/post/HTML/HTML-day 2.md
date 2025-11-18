---
title: "HTML-day2"
date: 2025-11-18T12:00:00+08:00
# 这一行必须是 false，并且不能有引号！
draft: false 
description: "这是我第二天学习HTML。"
---

大概内容：
	列表、标签语法、综合案例
<br>
<hr>
# （一）、列表标签
	1.作用：布局内容排列整齐的区域
	2.分类：无序、有序、定义
	3.无序列表：ul 嵌套多个 li ，内容不限制
	4.有序列表：ol 嵌套多个 li ，内容不限制
	5.定义列表：dl 只能嵌套多个 dt 和 dd ，dt和dd中不限制内

<br>
# （二）、表格

## 标签： table 嵌套 tr ,tr 嵌套 td/th
	1.table：表格
		1.border：边框粗细
	2.tr：行
	3.th：表头单元格
	4.td：内容单元格

## 表格结构标签：把内容划分区域
	1.thead：表格头部
	2.tbody：表格主题
	3.tfoot：表格底部

## 合并单元格：合并同类信息
	1.跨行合并：rowspan
	2.跨列合并：colspan
<br>
  
# （三）、表单

## 作用：收集用户信息	
<br>
## 输入 input
### input：type="属性"
	1.text：单行文本框
	2.password：密码框
	3.radio：单选框
	4.checkbox：多选框
	5.file：上传文件

### input：placehplder="文字"，提示输入
### input：name="label"，属于哪一个label
### input：checked ，默认值
###  input：multiple ，多文件上传

## 下拉菜单 select
### select嵌套多个option
	1.option:selected ，默认选择

## 文本域 textarea（css设计文本尺寸）
	1.rows
	2.cols
	3.右下角拖拽功能禁用

## 标签 label
	绑定文字和表单控件的关系，增大表单控件的范围
	for 对应的为 id

## 按钮 button
### button：type="属性"，这三个属性也能用input实现
	1.submit ，提交按钮
	2.reset ，重置按钮
	3.button ，普通按钮，配合js使用

### button：value="文字"
### 放入（form action=“地址”）（/form）标签才能使用

# （四）、div和span标签和字体实体
## 无语义，布局网页结构
	1.div：独占一行，又叫大盒子
	2.span：不换行，又叫小盒子
## 字符实体
	1.&nbsp：空格
	2.&lt：<
	3.&gt: >
	

# （五）、自己找一个网站做综合案例
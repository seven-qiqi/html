# HTML学习总结

## 		一、HTML是什么

​				**HTML**是超文本标记语言(**HyperText Markup Language**)的缩写，是构建web的工具。它不是一门编程语言，而是一种**定义内容结构的标记语言**。

​				**在浏览器中看到的任何网页背后都是一个 HTML 文档，只要在网页上点击鼠标右键->查看源代码（用控制台工具也可）就可看到**。				

## 		二、HTML文档结构

​				HTML 使用"标记"（markup）来注明文本、图片和其他内容，以便于在浏览器中显示。HTML 标记包含一些规定的"元素"如 <head>，<title>，<body>，<header>，<footer> 等等。

​				而HTML就是由一个个元素组成，每个元素则由一对tag构成。

​				例如:

```
        <html>
            <head>
                <title>HTML学习总结</title>
            </head>
            <body>
              网页内容
            </body>
        </html>
```

			标签<head></head>之间的文本是头部信息，在<title></title>之间的文本是文档标题，会显示在浏览器的窗口的标题栏。<body>	</body>之间的文本是正文。

## 	三、基础的tag

#### 		1.一些常用的tag

		<p></p> 可以用来定义段落。
		
		<br />可以用来在文本间换行。
		
		<hi></hi>(i表示1-6) 可以用来控制标题的大小。
		
		<a href=“URL”></a> 用来定义超链接，也可以用来对网页内进行跳转(锚点)。
		
		<img src="xxx" width="xx" height="xx" alt="xxx"/>用来定义图像，其中src表示图像的地址，width表示图像宽度，height表示图像高度，alt表示图像的代替文字。
		
		./表示该html文件所在的当前目录。
	
		../表示该html文件的上一层目录。
	
		images/表示该html文件下一层目录。
	
		../images/表示回到上一层目录，然后再进入images目录。

#### 		2.列表

 			无序列表用<ul><li></li></ul>表示。
 	
 				属性：    type
 				属性值：  列表前的符号	
 				disc     实心原点  
 				circle　　符号为空心圆
 				square　 符号为方形
 			例如:
 			    <ul type="disc">
 	         		<li>游戏</li>
 	         		<li>动漫</li>
 	         		<li>小说</li>
 	     		</ul>

​		  	 有序列表使用数字或字母系统来组织列表里包含的信息。有序列表可以使用数字(默认)、大写字母、小写字母、大写罗马数字和小写罗马数字排列项目。

​					属性       			属性值             				说明

​					type   		1、 a 、 A、i、I   	 用来设置项目前面的标记

​					start     				数值             	排序的起点数值

​				例如:

		<ol type="1" start="2">
	         <li>游戏</li>
	         <li>动漫</li>
	         <li>小说</li>
	     </ol>
	     <ol type="a">
	         <li>游戏</li>
	         <li>动漫</li>
	         <li>小说</li>
	     </ol>
	     <ol type="A">
	         <li>游戏</li>
	         <li>动漫</li>
	         <li>小说</li>
	     </ol>
	     <ol type="i">
	         <li>游戏</li>
	         <li>动漫</li>
	         <li>小说</li>
	     </ol>
	     <ol type="I">
	         <li>游戏</li>
	         <li>动漫</li>
	         <li>小说</li>
	     </ol>
#### 			3.表格

​				表格由 <table> 标签以及一个或多个 tr、th或td 元素组成。

​				单元格可以包含文本、图片、列表、段落、表单、水平线、表格等等。	

#### 			4.form表单

​				表单使用标签（<form>）定义。它主要负责获取用户填写的数据，并通过浏览器向服务器传送数据。

​				属性           说明

​				name          表单的名称

​				action         表单提交地址

​				method      表单数据提交的方式 （get:在url地址上面传送参数到服务器,post：在后台传送参数到服务器）

​				enctype      MIME类型       

​				target        打开方式（_blank:在一个新的窗口打开 _self:在相同的框架中调入文档 _top:把文档调入原来的最顶部的浏览器窗口中）

​	
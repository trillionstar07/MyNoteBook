#### 一、分析结构

本案例实现比较简单，根据下载好的素材结合实际效果图，可以看出使用一个外面的`<div>`盒子设置好背景，再将素材放置到内部的`<div>`盒子之中

#### 二、样式

1. 给外层的盒子设置宽度高度与贝尔经图像样式，背景图像沿水平方向平铺

2. 给里面的盒子设置宽度高度，背景图像设为不平铺，但内部盒子和外盒子的左边和上边留出一定空间

#### 三、开始制作

1. 打开Dreamweaver2021，新建一个HTML5格式文件，并添加title

2. 开始搭建架构,并将素材引入到对应位置
3. 引入css样式

**代码**

<!doctype html>
<html>
<head>
<meta charset="UTF-8">
<title>咖啡店</title>
	<style>
		.out{
			width:900px;
			height: 344px;
			background: url("bg.png") repeat-x;
			margin: 0 auto;
		}
		.in{
			width: 900px;
			height: 344px;
			background: url("coffee.png") no-repeat 42px 30px;
		}

	</style>
</head>
<body>
	<div class="out">
		<div class="in">
		</div>
	</div>
</body>
</html>
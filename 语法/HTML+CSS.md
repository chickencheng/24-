[HTML +CSS 语法](https://blog.csdn.net/CSSAJBQ_/article/details/123282888?ops_request_misc=&request_id=&biz_id=102&utm_term=html%E8%AF%AD%E6%B3%95&utm_medium=distribute.pc_search_result.none-task-blog-2~all~sobaiduweb~default-8-123282888.142^v100^pc_search_result_base4&spm=1018.2226.3001.4187)
## HTML

### 1.html基本结构

```html
<!DOCTYPE html>   声明当前的html文档是  html5
<html></html>    根标签（根节点） 一个网页中只有一个
<head></head>  头部标签  放页面的一些描述信息  
<meta>   描述  charset="UTF-8"  告诉浏览器这个文档编码格式是UTF-8

<title></title>     告诉浏览器 当前网页的标题
<body></body>     主体标签  浏览器主要窗口的内容  都放在body标签内  

```

### 2.标签

标签分类

​ 单标签 <标签名>

​ 双标签 <标签名>内容</标签名>

标签

​ [标题标签](https://so.csdn.net/so/search?q=%E6%A0%87%E9%A2%98%E6%A0%87%E7%AD%BE&spm=1001.2101.3001.7020) h1-h6 段落标签 p 换行 br 水平线 hr

##### 文本格式化 标签

​ 加粗 b trong

​ 倾斜 i em

​ 下划线 u [ins](https://so.csdn.net/so/search?q=ins&spm=1001.2101.3001.7020)

​ 删除线 s del

##### 字体标签 font

```html
 字体标签  font
    双标签
     属性
        颜色 color  
            color = "颜色值"  定义颜色
        大小  size 
            sise = "1-7"   定义字体的大小 
    <font color = "red">这是第一行的文字</font>
    <font size = "1">这是第二行的文字</font>
    <font size = "6" color = "blue">这是第三行的文字</font>

```

##### div span 无语义标签 （盒子）

特点：

div 独立一行 [块级元素](https://so.csdn.net/so/search?q=%E5%9D%97%E7%BA%A7%E5%85%83%E7%B4%A0&spm=1001.2101.3001.7020)

span 一行可以显示多个 行内元素

##### img 图片标签

```html
 作用 : 在页面当中引入一张图片
    属性 ： 
        1. src="图片的路径"   img的必备属性 
        2. alt="对图片的描述词"  只有在图片加载失败的时候显示
        3. title="图片的提示"  只有在鼠标悬停的时候显示  所有标签都可以有title属性
        4. width="数字px"   设置图片的宽度 如果只设置一个宽度 没有设置高度的时候 浏览器会自动设置同比例的高度
        5. height="数字px"  设置图片的高度   
        6. border="数字px"  设置图片的边框
<img src="ys.jpg" alt="耶稣" title="耶稣保佑我" width="800px" height="200px" border="1px">
```

路径关系 重点

​ 绝对路径

​ \1. 本地绝对路径

​ \2. 外网相对路径

​ 相对路径

​ 1.同级

​ 2.上级

​ 3.下级

```html
 路径
        绝对路径
            1.本地绝对路径(当前计算机盘符出发，一直找到对应的目标)
             <img src="F:/广州叩丁狼前端211011班（37期）/01-html+css/day01-html第一天/02-课堂代码/images/ys.jpg">
            2.外网绝对路径
            http...
			<img src="http://qqpublic.qpic.cn/qq_public/0/0-893702753-88308B4DB55AB4604F36296B3F6403F3/0?fmt=jpg&size=55&h=506&w=900&ppv=1.jpg" alt="">

        相对路径(重点)  
            1.  图片和页面在同一级目录的时候  直接写图片名  ./图片名
            2.  图片在页面的上一级目录   ../ 跳到上一级目录
            3.  图片在页面的下一级目录   文件夹名/图片名

        细节:
            1. 精确到图片名.后缀
            2. 具体的路径正不正确 
            3. 相对路径一定要找准位置关系
    
   
```

##### 超链接 a标签

锚点 特殊字符

```html
    超链接  a   双标签
    作用 : 点击之后 跳转到另外的位置
    <a href="你要跳转的位置">内容</a>
    属性: 
        1. href="你要跳转的位置(路径)"
        2. target="_self或者_blank"  超链接点击之后打开新链接的方式
            _self默认值 在当前标签页打开新页面
            _blank 新开一个标签窗口打开新页面

    <a href="http://www.baidu.com">百度首页</a>
    <a href="./14-路径.html" >刚才的页面</a>
    
    
  锚点  语法: <a href="#锚点名"></a>
	作用：点击之后页面滑到id名对应的标签的位置
   	<a href="#test1"></a>
    <p id="test1"></p>
```

##### 特殊字符：

大于号 >； 小于号<； 空格 ； …

#### 

##### 列表

无序列表 ul > li

有序列表 ol > li

自定义列表 dl > dt dd

```html
	  
 ☞ 无序列表(unordered-list)
	  <ul>
          <li> 列表项	</li>
          <li> 列表项	</li>
          ...
	  </ul>
	总结：
		 1. ul列表必须直接包含的标签是li
		 2. 在li标签中可以包含其他任何标签
		 3. 在展示数据的时候没有先后顺序的要求


  ☞ 有序列表： (order-list)
		<ol>
            <li> </li>
            <li> </li>
            <li> </li>
		</ol>

	 总结：
	     1. 有序列表在展示数据的时候是按照一定的顺序显示的
		 2. 有序列表在用法上与无序列表一样。


  ☞ 自定义列表(defined-list)

	<dl>
        <dt> </dt>
        <dd> 列表项 </dd>
        <dd> 列表项 </dd>
        <dd> 列表项 </dd>
	</dl>

	总结：
		一般在网页的结尾处会使用该列表


```

##### 表格 table

```html
	  ◆ 表格中的属性级其他标签介绍：
		   1. border属性： 设置边框

		   2. width属性： 改变宽度

		   3. height属性： 改变高度
		
	       4. 去掉td与td之间的距离  cellspacing的默认是2 

		   5. 设置内容居中显示  align: left | center  | right
			   ◆如果希望表格中的内容对齐，那么将align属性设置给tr或者td
			   ◆如果将align属性设置给table，只能改变table整体的对齐方式，不会影响内容的对齐方式
		
		   6. 如果希望给表格设置表头，那么请使用th标签替代td标签，th在表格中就是表示表头，默认实现文字居中加粗显示
	
		    7. 设置背景颜色属性： bgcolor="颜色"；

		  	8. 设置表格的标题   <caption> </caption>

<table border="1" width="400" height="400"  cellspacing="0" align="center"  bgcolor="pink">
    <caption > 人员信息表</caption>
    <thead> 
        <tr>
            <th>姓名</th>
            <th>英语</th>
            <th>语文</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>张三</td>
            <td>39</td>
            <td>80</td>
        </tr>
    </tbody>
    <tfoot>
         <tr>
            <td>平均分</td>
            <td></td>
            <td></td>
        </tr>
    </tfoot>
</table>
```

##### 表单 form

```html
 <form action="xxx.php">
文本输入框
        <input type="text" >
密码框
        <input type="password" >
        <br>
       
单选框
        <input type="radio" name="sex">男
        <input type="radio" name="sex">女
        <br> 
复选框 
        <input type="checkbox" name="" id="">男
        <input type="checkbox">女<br>
按钮
       
        <input type="button" value="按钮"><br>
        
 大按钮       
        <button >大按钮 </button> <br>
       
提交按钮
        <input type="submit" value="提交按钮"><br>
重置按钮
        <input type="reset" value="重新填写"><br>
文件上传
        <input type="file" name="" id="">
        <br>
 input的name （名字）<br>
 value（值）属性<br>
        
        <input type="text" name="size" value="大">大
        <input type="text" name="size" value="小">小

 input的maxlength（字符串最大长度）属性<br>
        <input type="text" name="sex"  maxlength="3"><br>
 input的placeholder占位属性 <br>
       用户名： <input type="text" name="sex" placeholder="请输入用户名">
       密码： <input type="password" name="sex"placeholder="请输入密码"><br>
input的选中checked状态

       <input type="radio" name="sex"checked>男
        <input type="radio" name="sex">女<br>
  下拉选框  select标签和 selected当前显示的
        <select name="" id="">
                <option value="">1</option>
                <option value="">2</option>
                <option value="" selected>3</option>
                <option value="">4</option>
        </select><br>
  文本域
         <textarea name="" id="" cols="30" rows="10"></textarea>请输入文字
    </form>
```

## CSS

### 3.css

##### css概念

```
**CSS** 是层叠样式表 ( Cascading Style Sheets ) 的简称

CSS 主要用于设置 HTML 页面中的文本内容（字体、大小、对齐方式等）、图片的外形（宽高、边框样式、边距等）以及版面的布局和外观显示样式。

简单理解：1. HTML 主要做结构,显示元素内容.

         2. CSS 美化 HTML ,布局网页.
```

##### css语法规范

```
 1.选择器是用于指定 CSS 样式的 HTML 标签，花括号内是对该对象设置的具体样式
 2.属性和属性值以“键值对”的形式出现
 3.属性是对指定的对象设置的样式属性，例如字体大小、文本颜色等
 4.属性和属性值之间用英文“:”分开
 5.多个“键值对”之间用英文“;”进行区分
 例如：
    所有的样式，都包含在 <style> 标签内，表示是样式表。<style> 一般写到 </head> 上方
<head>
    <style>
        h4 {
             color: blue;    属性名：属性值；
             font-size: 100px;
            }
    </style>
</head>
```

##### 选择器

|基础选择器|作用|特点|使用情况|用法|
|---|---|---|---|---|
|标签选择器|可以选出所有相同的标签|不能差异化选择|较多|p { color : red }|
|类选择器|可以选出一个或者多个标签|可以根据需求选择|非常多|.nav { color : red }|
|id选择器|一次只能选择1个标签|ID属性只能在每个HTML文档出现1次|一般和js搭配1使用|#nav { color : red }|
|通配符选择器|选择所有的标签|选择太多，有的部分不需要|特殊情况使用|* { color ：red }|

### 4.字体属性

##### 字体大小 font-size：

```
CSS 使用 font-size 属性定义字体大小。 
语法：
    选择器 {  
          font-size: 数字px; 
   }
```

##### 字体粗细 font-weight：

```
CSS 使用 font-weight 属性设置文本字体的粗细。
font-weight: 单词/数值
 单词：       bold加粗   lighter细体  
 数值：       200细体  400正常大小 700加粗
 
 语法：
   选择器 {  
           font-weight:  bold； 字体粗细
           
   }
   
   或者
    选择器 {  
           font-weight:  700；
   }
   
   
```

##### 字体类型 font-family：

```
css使用 font-family 属性定义字体的类型 （宋体、微软雅黑）
语法：

  选择器{
	font-family:  'Microsoft Yahei'
}



```

##### 字体倾斜样式 font-style：

italic斜体 normal正常

```
语法：

选择器 {  
        font-style:  italic;
    }


```

##### 字体样式——综合写法 font

```
语法：

 font: 字体样式  字体粗细  字体大小/行高 字体家族;
 
 font:  italic 700 60px 宋体
```

##### 文字溢出隐藏

```css
 white-space: nowrap;
 overflow: hidden;
 text-overflow: ellipsis;
```

### 5. 文本属性

##### 文本对齐方式

```
属性用于设置元素内文本内容的水平对齐方式。
center居中  left左对齐  right右对齐

        text-align: center;

```

##### 文本修饰线 text-decoration：

```html

       	text-decoration：none；         无
		text-decoration：underline；    下划线
		text-decoration：overline；     上划线
		text-decoration: line-through； 文字删除线


```

##### 文本缩进 text indent

```
2种语法：
选择器 { 
        text-indent：20px;
    }
 选择器 { 
        text-indent：2em；
    }
em 是一个相对单位，就是当前元素（font-size) 1 个文字的大小
就是： 1em=当前文字大小 

比如：一个字符浏览器中文默认大小是16px 2个字符就是32px
也可以说是2em
```

### 6. css样式表：

##### 行内样式表（行内式）

在元素标签内部的 style 属性中设定 CSS 样式。适合于修改简单样式.

```
行内样式表（内联样式表）是在元素标签内部的 style 属性中设定 CSS 样式。适合于修改简单样式.
    语法：
        <div style="color: red; font-size: 12px;">青春不常在，抓紧谈恋爱</div>
    1.style 其实就是标签的属性
    在双引号中间，写法要符合 CSS 规范
    2.可以控制当前的标签设置样式
    3.由于书写繁琐，并且没有体现出结构与样式相分离的思想，所以不推荐大量使用，只有对当前元素添加简单样式的时候，可以考虑使用
    4.使用行内样式表设定 CSS，通常也被称为行内式引入
```

##### 内部样式表（嵌入式）

写到html页面内部. 是将所有的 CSS 代码抽取出来，单独放到一个

```html
 内部样式表（内嵌样式表）是写到html页面内部. 是将所有的 CSS 代码抽取出来，单独放到一个 <style> 标签中
    语法：
        <style>
            div {
            color: red;
            font-size: 12px;
            }
        </style>
    1.<style> 标签理论上可以放在 HTML 文档的任何地方，但一般会放在文档的<head>标签中
    2.通过此种方式，可以方便控制当前整个页面中的元素样式设置
    3.代码结构清晰，但是并没有实现结构与样式完全分离
    4.使用内部样式表设定 CSS，通常也被称为嵌入式引入，这种方式是我们练习时常用的方式
```

##### 外部样式表（链接式）

样式单独写到CSS 文件中，之后把CSS文件 使用 标签 引入到 HTML 页面中使用.

```html
实际开发都是外部样式表. 适合于样式比较多的情况. 核心是:样式单独写到CSS 文件中，之后把CSS文件引入到 HTML 页面中使用.
引入外部样式表分为两步：
1. 新建一个后缀名为 .css 的样式文件，把所有 CSS 代码都放入此文件中。
2. 在 HTML 页面中，使用<link> 标签引入这个文件。
语法：
    <link rel="stylesheet"  href="css文件路径">
```

### 7.css三大特性

层叠性 ：多种样式的叠加----就近原则

继承性：子承父业

优先级：概念：

定义CSS样式时，经常出现两个或更多规则应用在同一元素上，此时，

- 选择器相同，则执行层叠性
    
- 选择器不同，就会出现优先级的问题。
    
    权重公式
    

|标签选择器|计算权重公式|
|---|---|
|继承或者 *|0,0,0,0|
|每个元素（标签选择器）|0,0,0,1|
|每个类，伪类|0,0,1,0|
|每个ID|0,1,0,0|
|每个行内样式 style=“”|1,0,0,0|
|每个!important 重要的|∞ 无穷大|

权重叠加

- div ul li ------> 0,0,0,3
- .nav ul li ------> 0,0,1,2
- a:hover -----—> 0,0,1,1
- .nav a ------> 0,0,1,1

网页布局的本质 --盒子的摆放

### 8.盒子模型

![img](https://img-blog.csdnimg.cn/img_convert/c01441f8041e26a46f5c3326745d31af.png)

1. 盒子模型= 外边距（margin） + 边框（border） + 内边距（padding） + 内容（content）
2. 盒子里面的文字和图片等元素是 内容区域
3. 盒子的厚度 我们成为 盒子的边框
4. 盒子内容与边框的距离是内边距（类似单元格的 cellpadding)
5. 盒子与盒子之间的距离是外边距（类似单元格的 cellspacing）

##### 盒子边框（border）

边框的样式：

- none：没有边框即忽略所有边框的宽度（默认值）
- solid：边框为单实线(最为常用的)
- dashed：边框为虚线
- dotted：边框为点线

1边框综合设置

```css
border : border-width || border-style || border-color 
```

例如：

```css
 border: 1px solid red;  没有顺序  
```

2 盒子边框写法总结表

很多情况下，我们不需要指定4个边框，我们是可以单独给4个边框分别指定的。

|上边框|下边框|左边框|右边框|
|:--|:--|:--|:--|
|border-top-style:样式;|border-bottom-style:样式;|border-left-style:样式;|border-right-style:样式;|
|border-top-width:宽度;|border- bottom-width:宽度;|border-left-width:宽度;|border-right-width:宽度;|
|border-top-color:颜色;|border- bottom-color:颜色;|border-left-color:颜色;|border-right-color:颜色;|
|border-top:宽度 样式 颜色;|border-bottom:宽度 样式 颜色;|border-left:宽度 样式 颜色;|border-right:宽度 样式 颜色;|

3 表格的细线边框

通过表格的`cellspacing="0"`,将单元格与单元格之间的距离设置为0，

- 但是两个单元格之间的边框会出现重叠，从而使边框变粗
    
- 通过css属性：
    
    ```css
    table{ 
    border-collapse:collapse; 
    }  
    ```
    
    - collapse 单词是合并的意思
    - border-collapse:collapse; 表示相邻边框合并在一起。

```css
<style>
	table {
		width: 500px;
		height: 300px;
		border: 1px solid red;
	}
	td {
		border: 1px solid red;
		text-align: center;
	}
	table, td {
		border-collapse: collapse;  /*合并相邻边框*/
	}
</style>
```

内边距（padding）

1 内边距：

​ padding属性用于设置内边距。 **是指 边框与内容之间的距离。**

2 设置

|属性|作用|
|---|:--|
|padding-left|左内边距|
|padding-right|右内边距|
|padding-top|上内边距|
|padding-bottom|下内边距|

当我们给盒子指定padding值之后， 发生了2件事情：

1. 内容和边框 有了距离，添加了内边距。
2. 盒子会变大了。

我们分开写有点麻烦，我们可以不可以简写呢？

|值的个数|表达意思|
|---|---|
|1个值|padding：上下左右内边距;|
|2个值|padding: 上下内边距 左右内边距 ；|
|3个值|padding：上内边距 左右内边距 下内边距；|
|4个值|padding: 上内边距 右内边距 下内边距 左内边距 ；|

4 内盒尺寸计算（元素实际大小）

- 宽度
    
    Element Height = content height + padding + border （Height为内容高度）
    
- 高度
    
    Element Width = content width + padding + border （Width为内容宽度）
    
- 盒子的实际的大小 = 内容的宽度和高度 + 内边距 + 边框
    

5 padding不影响盒子大小情况

> 如果没有给一个盒子指定宽度， 此时，如果给这个盒子指定padding， 则不会撑开盒子。

##### 外边距（margin）

1 外边距

​ margin属性用于设置外边距。 margin就是控制**盒子和盒子之间的距离**

2 设置：

|属性|作用|
|---|:--|
|margin-left|左外边距|
|margin-right|右外边距|
|margin-top|上外边距|
|margin-bottom|下外边距|

margin值的简写 （复合写法）代表意思 跟 padding 完全相同。

3 块级盒子水平居中

- 可以让一个块级盒子实现水平居中必须：
    - 盒子必须指定了宽度（width）
    - 然后就给**左右的外边距都设置为auto**，

实际工作中常用这种方式进行网页布局，示例代码如下：

```css
.header{ width:960px; margin:0 auto;}
```

常见的写法，以下下三种都可以。

- margin-left: auto; margin-right: auto;
- margin: auto;
- margin: 0 auto;

4 文字居中和盒子居中区别

1. 盒子内的文字水平居中是 text-align: center, 而且还可以让 行内元素和行内块居中对齐
2. 块级盒子水平居中 左右margin 改为 auto

```css
text-align: center; /*  文字 行内元素 行内块元素水平居中 */
margin: 10px auto;  /* 块级盒子水平居中  左右margin 改为 auto 就阔以了 上下margin都可以 */
```

5 插入图片和背景图片区别

1. 插入图片 我们用的最多 比如产品展示类 移动位置只能靠盒模型 padding margin
2. 背景图片我们一般用于小图标背景 或者 超大背景图片 背景图片 只能通过 background-position

```css
 img {  
		width: 200px;/* 插入图片更改大小 width 和 height */
		height: 210px;
		margin-top: 30px;  /* 插入图片更改位置 可以用margin 或padding  盒模型 */
		margin-left: 50px; /* 插入当图片也是一个盒子 */
	}

 div {
		width: 400px;
		height: 400px;
		border: 1px solid purple;
		background: #fff url(images/sun.jpg) no-repeat;
		background-position: 30px 50px; /* 背景图片更改位置 我用 background-position */
	}
```

6 清除元素的默认内外边距(重要)

为了更灵活方便地控制网页中的元素，制作网页时，我们需要将元素的默认内外边距清除

代码：

```css
* {
   padding:0;         /* 清除内边距 */
   margin:0;          /* 清除外边距 */
}
```

注意：

- 行内元素为了照顾兼容性， 尽量只设置左右内外边距， 不要设置上下内外边距。

7 外边距合并

使用margin定义块元素的**垂直外边距**时，可能会出现外边距的合并。

(1). 相邻块元素垂直外边距的合并

- 当上下相邻的两个块元素相遇时，如果上面的元素有下外边距margin-bottom
- 下面的元素有上外边距margin-top，则他们之间的垂直间距不是margin-bottom与margin-top之和
- **取两个值中的较大者**这种现象被称为相邻块元素垂直外边距的合并（也称外边距塌陷）。

**解决方案：尽量给只给一个盒子添加margin值**。

(2). 嵌套块元素垂直外边距的合并（塌陷）

- 对于两个嵌套关系的块元素，如果父元素没有上内边距及边框
- 父元素的上外边距会与子元素的上外边距发生合并
- 合并后的外边距为两者中的较大者

**解决方案：**

1. 可以为父元素定义上边框。
2. 可以为父元素定义上内边距
3. 可以为父元素添加overflow:hidden。

还有其他方法，比如浮动、固定、绝对定位的盒子不会有问题，后面咱们再总结。。。

### 9. 盒子模型布局稳定性

- 学习完盒子模型，内边距和外边距，什么情况下用内边距，什么情况下用外边距？
    - 大部分情况下是可以混用的。 就是说，你用内边距也可以，用外边距也可以。 你觉得哪个方便，就用哪个。

我们根据稳定性来分，建议如下：

按照 优先使用 宽度 （width） 其次 使用内边距（padding） 再次 外边距（margin）。

```
  width >  padding  >   margin   
```

- 原因：
    - margin 会有外边距合并 还有 ie6下面margin 加倍的bug（讨厌）所以最后使用。
    - padding 会影响盒子大小， 需要进行加减计算（麻烦） 其次使用。
    - width 没有问题（嗨皮）我们经常使用宽度剩余法 高度剩余法来做。

##### 去掉列表默认的样式

无序和有序列表前面默认的列表样式，在不同浏览器显示效果不一样，而且也比较难看，所以，我们一般上来就直接去掉这些列表样式就行了。 代码如下

```css
li { list-style: none; }
```

### 10. 拓展其他样式

##### 1 圆角边框

在 CSS3 中，新增了圆角边框样式，这样我们的盒子就可以变圆角了。

border-radius 属性用于设置元素的外边框圆角。

语法：

```css
 border-radius:length;    
```

- 参数值可以为数值或百分比的形式
- 如果是正方形，想要设置为一个圆，把数值修改为高度或者宽度的一半即可，或者直接写为 50%
- 该属性是一个简写属性，可以跟四个值，分别代表左上角、右上角、右下角、左下角
- 分开写：border-top-left-radius、border-top-right-radius、border-bottom-right-radius 和border-bottom-left-radius
- 兼容性 ie9+ 浏览器支持, 但是不会影响页面布局,可以放心使用

##### 2 盒子阴影

CSS3 中新增了盒子阴影，我们可以使用 box-shadow 属性为盒子添加阴影。  
语法：

```css
 box-shadow: h-shadow v-shadow blur spread color inset; 
```

[外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传(img-9TkOz0X0-1646389446725)(F:/叩丁狼/1.html+css/day05-第三天/01-课堂笔记/assets/1571541874805.png)]

##### 3 文字阴影

在 CSS3 中，我们可以使用 text-shadow 属性将阴影应用于文本。  
语法：

```css
 text-shadow: h-shadow v-shadow blur color;
```

[外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传(img-D0yfctkX-1646389446725)(F:/叩丁狼/1.html+css/day05-第三天/01-课堂笔记/assets/1571541954222.png)]

##### 4 过渡

```
transition： all  1s  过渡所需要的时间
```

##### 5 缩放属性

```
transform： scale（缩放值）

例如
transform： scale（1.5） 放大1.5倍

```

##### 6 contenteditable 内容可编辑

```css

给元素加个contenteditable=true就可以当输入框
语法：
<element contenteditable="true|false">

<p contenteditable="true">这是一个可编辑的段落。</p>
```

### 11 .CSS 布局的三种机制

> 网页布局的核心——就是**用 CSS 来摆放盒子**。

CSS 提供了 **3 种机制**来设置盒子的摆放位置，分别是**普通流**（标准流）、**浮动**和**定位**，其中：

1. **普通流**（标准流）
    
    块级元素**会独占一行，**从上向下**顺序排列；
    
    - 常用元素：div、hr、p、h1~h6、ul、ol、dl、form、table
    
    行内元素**会按照顺序，**从左到右**顺序排列，碰到父元素边缘则自动换行；
    
    - 常用元素：span、a、i、em等
    
    行内块元素 ，支持宽高，从左到右排列，受空格影响，不独占一行；
    
    - 常用元素：img、input、textarea
2. **浮动**
    
    - 让盒子从普通流中**浮**起来,主要作用让多个块级盒子一行显示。
3. **定位**
    
    - 将盒子**定**在浏览器的某一个**位**置——CSS 离不开定位，特别是后面的 js 特效。

### 12.浮动 float

浮动是什么？为什么要用浮动？

让盒子从普通流中**浮**起来,主要作用让多个块级盒子一行显示

因为一些网页布局要求，标准流不能满足需要，所以要浮动来完成网页的布局

**浮动特点：**

脱离标准流，漂浮在标准流上面，不受标准流影响 俗称 ”脱标“

不占有原来位置

float属性会改变元素display属性，具有行内块的特点: 默认由内容撑开宽高，也可手动设置宽高，一行可以显示多个 ，类似转换为了行内块，但是元素之间**没有空白缝隙**

**注意： 浮动的元素互相贴靠一起的，但是如果父级宽度装不下这些浮动的盒子， 多出的盒子会另起一行对齐**

浮动 CSS语法：

```css
选择器 {
	float：none；  元素不浮动（默认值）
	float：left；  元素向左浮动
	float：right； 元素向右浮动
}
```

### 13.清除浮动

**1 为什么要清除浮动**

1. 父级没高度
2. 子盒子浮动了
3. 影响下面布局了，我们就应该清除浮动了。

**2.清除浮动方法**

1.隔墙法（额外标签法）

```html
<div style="clear:both;"></div> //W3C推荐做法 在浮动元素末尾添加一个空标签
```

2.父级设置 overflow属性 方法

```css
可以给父级添加： overflow为 hidden || auto || scroll  都可以实现。
```

3.使用after伪元素清除浮动

```css
.clearfix::after { 
	content:"";
	display:block;
	height:0;
	clear:both;
	visibility:hidden;
	}
.clearfix{
    *zoom:1;
}    /*IE6、7专有*/
```

4.使用双伪元素清除浮动

```css
.clearfix::before,.clearfix::after{
	content:"";
	display:table;
}
.clearfix::after{
	clear:both;
}
.clearfix{
	*zoom:1;
}
```

### 14.元素的显示与隐藏

1. display 属性

```css
display: none;    //隐藏元素，并且不占原来的位置
display: block;   //显示隐藏的元素
```

2. visibility 属性

```css
visibility: hidden;   //隐藏元素，元素隐藏后继续占有原先的位置
visibility: visible;  //元素可视
```

3. overflow 属性
    
    overflow 属性指定了 如果内容溢出了元素框（即超过了元素的指定高度和宽度），会发生什么事
    

```css
overflow: visible;  //显示内容并且超出的内容
overflow: hidden;   //隐藏超出的部分
overflow: scroll;   //使用滚动条显示内容
verflow:auto;       // 如果有超出的部分，则使用滚动条，如果没有，则不使用
```

### 15.css用户界面样式

##### 鼠标样式 cursor 属性

音标 英[ˈkɜːsə®] 鼠标悬停的时候显示对应的样式

cursor: defult; 显示鼠标 || pointer 小手 || move 移动 || text 文本—显示编辑光标 || not-allowed 文本----显示禁止符

- 我是小白
- 我是小手
- 我是移动
- 我是文本
- 我是文本

##### 轮廓 outline

```css
 outline : outline-color ||outline-style || outline-width 
```

但是 一般我们都是去掉这个样式的

```css
 outline: 0;   或者  outline: none;
```

##### 防止拖拽文本域 resize

resize：none 这个单词可以防止 火狐 谷歌等浏览器随意的拖动 文本域。

右下角可以拖拽：

右下角不可以拖拽：

### 16.vertical-align 垂直对齐

vertical-align 不影响块级元素中的内容对齐，它只针对于 行内元素或者行内块元素，特别是行内块元素， **通常用来控制图片/表单与文字的对齐**。

```css
vertical-align : baseline  基线对齐
				middle   垂直居中
				top      顶部对齐
                 bottom    底部对齐
```

##### **去除图片底侧空白缝隙**

有个很重要特性你要记住： 图片或者表单等行内块元素，默认他的底线会和父级盒子的基线对齐。这样会造成一个问题，就是图片底侧会有一个空白缝隙。

解决办法

第一种： 给img 设置 vertical-align：middle || top等等 让图片不要和基线对齐。

第二种：给img 添加 display：block; 转换为块级元素。

### 17.**溢出文字隐藏 **

white-space：设置或检索对象内文本显示方式。通常我们使用于强制一行显示内容

normal : 　默认处理方式  
nowrap : 　强制在同一行内显示所有文本，直到文本结束或者遭遇br标签对象才换行。

text-overflow 文字溢出

标示对象内文本的溢出

text-overflow : clip 裁切 || ellipsis 显示省略标记（…）

注意一定要首先强制一行内（nowrap不换行）显示，再次和overflow属性 搭配使用

单行文字超出 ，以省略号显示

```css
 .box { 	
             width:300px;
            /* 单行文字超出 ，以省略号显示
            1. 强制让文字不换行
             */
             white-space: nowrap;
             /* 2. 让超出部分隐藏 */
             overflow: hidden;
             /* 3.超出部分用省略号表示 */
             text-overflow: ellipsis;
        }
```

### 18.精灵技术（sprite）

精灵图 雪碧 小妖精

什么是精灵图 ？

​ 一张图片里 有很多小小的小图片

​ 为什么使用精灵图？

​ 减少服务器的访问次数，提高性能

​ 怎么用精灵图？

​ 1. 精灵图中小图标的大小,量出展示的图片的大小

​ 2. 引入到页面(背景图)

​ 3. 调整背景定位

```css
 .box {
            /* 1. 量出展示的图片的大小 */
            width: 60px;
            height: 60px;
            /* border: 1px solid red; */
            /* 2. 引入到页面(背景图) */
            background-image: url('./昨日作业/images/index.png');
            /* 3. 调整背景定位 */
            background-position: -183px 3px;

        }
```

### 19.三角形

```css
 .box1 {
            /* width: 50px;
            height: 50px; */
            width: 0;
            height: 0;
            border: 100px solid transparent;
            border-right: 100px solid green;
           /* 生成三角形
            1. 需要宽高为0的div
            2. 设置边框的大小 ，边框的大小会决定三角的大小， 所有边框的颜色设置为透明色transparent
            3.单独设置需要的三角形 （方向）
           
            */
        }
```

```css
/*直角三角形*/
.box2{
            width: 0;
            height: 0;
            border:120px solid transparent ;
            border-bottom: 240px solid red;
            border-right: 0;

        }
```

### 20. [html5新特性总结](https://www.cnblogs.com/binguo666/p/10928907.html)

html5总的来说比html4多了十个新特性，但其不支持ie8及ie8以下版本的浏览器

一、语义标签

二、增强型表单

三、视频和音频

四、Canvas绘图

五、SVG绘图

六、地理定位

七、拖放API

八、WebWorker

九、WebStorage

十、WebSocket

**一、语义标签**

html5语义标签，可以使开发者更方便清晰构建页面的布局

|标签|描述|
|---|---|
||定义了文档的头部区域|
||定义了文档的尾部区域|
||定义文档的导航|
||定义文档中的节|
||定义文章|
||定义页面以外的内容|
||定义用户可以看到或者隐藏的额外细节|
||标签包含details元素的标题|
||定义对话框|
||定义自包含内容，如图表|
||定义文档主内容|
||定义文档的主内容|
||定义日期/时间|

![img](https://img-blog.csdnimg.cn/img_convert/5c57e7d5927e6c0e2d4178dd8260bfb8.png)

**二、增强型表单**

html5修改一些新的input输入特性，改善更好的输入控制和验证

|输入类型|描述|
|---|---|
|color|主要用于选取颜色|
|date|选取日期|
|datetime|选取日期(UTC时间)|
|datetime-local|选取日期（无时区）|
|month|选择一个月份|
|week|选择周和年|
|time|选择一个时间|
|email|包含e-mail地址的输入域|
|number|数值的输入域|
|url|url地址的输入域|
|tel|定义输入电话号码和字段|
|search|用于搜索域|
|range|一个范围内数字值的输入域|

html5新增了五个表单元素

|datalist|用户会在他们输入数据时看到域定义选项的下拉列表|
|---|---|
|progress|进度条，展示连接/下载进度|
|meter|刻度值，用于某些计量，例如温度、重量等|
|keygen|提供一种验证用户的可靠方法生成一个公钥和私钥|
|output|用于不同类型的输出比如尖酸或脚本输出|

html5新增表单属性

|属性|描述|
|---|---|
|placehoder|输入框默认提示文字|
|required|要求输入的内容是否可为空|
|pattern|描述一个正则表达式验证输入的值|
|min/max|设置元素最小/最大值|
|step|为输入域规定合法的数字间隔|
|height/wdith|用于image类型input标签图像高度/宽度|
|autofocus|规定在页面加载时，域自动获得焦点|
|multiple|规定input元素中可选择多个值|

**三、音频和视频**

html5提供了音频和视频文件的标准，既使用元素。

音频：

autoplay 自动播放（谷歌浏览器不支持）

controls 是否显不默认播放控件

loop 循环播放 loop = 2 就是循环2次 loop 或者 loop = “-1” 无限循环

```css
<audio controls>    //controls属性提供添加播放、暂停和音量控件。
  <source src="horse.ogg" type="audio/ogg">
  <source src="horse.mp3" type="audio/mpeg">
您的浏览器不支持 audio 元素。        //浏览器不支持时显示文字
</audio>
```

视频：

autoplay 自动播放（谷歌浏览器不支持，需要再设置muted属性实现静音播放）

controls 是否显示默认播放控件

loop 循环播放

width 设置播放窗口宽度

height 设置播放窗口的高度

```css
<video width="320" height="240" controls>
  <source src="movie.mp4" type="video/mp4">
  <source src="movie.ogg" type="video/ogg">
您的浏览器不支持Video标签。
</video>
```

**四、Canvas绘图**

[https://www.runoob.com/w3cnote/html5-canvas-intro.html](https://www.runoob.com/w3cnote/html5-canvas-intro.html)

**五、SVG绘图**

什么是SVG?

SVG指可伸缩矢量图形

SVG用于定义用于网络的基于矢量的图形

SVG使用XML格式定义图形

SVG图像在放大或改变尺寸的情况下其图形质量不会有损失

SVG是万维网联盟的标准

SVG的优势

与其他图像格式相比，是哟个SVG的优势在于：

SVG图像可通过文本编译器来创建和修改

SVG图像可被搜索、索引、脚本化或压缩

SVG是可伸缩的

SVG图像可在任何的分辨率下被高质量的打印

SVG可在图像质量不下降的情况下被放大

SVG与Canvas区别

*SVG适用于描述XML中的2D图形的语言

*Canvas随时随地绘制2D图形（使用javaScript）

*SVG是基于XML的，意味这可以操作DOM，渲染速度较慢

*在SVG中每个形状都被当做是一个对象，如果SVG发生改变，页面就会发生重绘

*Canvas是一像素一像素地渲染，如果改变某一个位置，整个画布会重绘。

|Canvas|SVG|
|---|---|
|依赖分辨率|不依赖分辨率|
|不支持事件处理器|支持事件处理器|
|能够以.png或.jpg格式保存结果图像|复杂度会减慢搞渲染速度|
|文字呈现功能比较简单|适合大型渲染区域的应用程序|
|最合适图像密集的游戏|不适合游戏应用|

**六、地理定位**

使用getCurrentPosition()方法来获取用户的位置。以实现“LBS服务”

```css
 <div id="demo"></div>
    <script>
        var x = document.getElementById("demo");

        function getLocation() {
            if (navigator.geolocation) {
                navigator.geolocation.getCurrentPosition(showPosition);
            } else {
                x.innerHTML = "Geolocation is not supported by this browser.";
            }
        }
      

        function showPosition(position) {
            x.innerHTML = "Latitude: " + position.coords.latitude +
                "<br />Longitude: " + position.coords.longitude;
        }
        
        getLocation();
        // Latitude: 23.1334117
        // Longitude: 113.3720223 获取当前位置经纬度
    </script>
```

**七、拖放API**

拖放是一种常见的特性，即捉取对象以后拖到另一个位置。

在html5中，拖放是标准的一部分，任何元素都能够拖放。

```
<div draggable="true"></div>
```

当元素拖动时，我们可以检查其拖动的数据。

```
<div draggable="true" ondragstart="drag(event)"></div>
<script>
function drap(ev){
    console.log(ev);
}
</script>
```

|拖动生命周期|属性名|描述|
|---|---|---|
|拖动开始|ondragstart|在拖动操作开始时执行脚本|
|拖动过程中|ondrag|只要脚本在被拖动就运行脚本|
|拖动过程中|ondragenter|当元素被拖动到一个合法的防止目标时，执行脚本|
|拖动过程中|ondragover|只要元素正在合法的防止目标上拖动时，就执行脚本|
|拖动过程中|ondragleave|当元素离开合法的防止目标时|
|拖动结束|ondrop|将被拖动元素放在目标元素内时运行脚本|
|拖动结束|ondragend|在拖动操作结束时运行脚本|

**八、Web Worker**

Web Worker可以通过加载一个脚本文件，进而创建一个独立工作的线程，在主线程之外运行。

基本使用：

Web Worker的基本原理就是在当前javascript的主线程中，使用Worker类加载一个javascript文件来开辟一个新的线程，

起到互不阻塞执行的效果，并且提供主线程和新县城之间数据交换的接口：postMessage、onmessage。

javascript:

```css
//worker.js
onmessage =function (evt){
  var d = evt.data;//通过evt.data获得发送来的数据
  postMessage( d );//将获取到的数据发送会主线程
}
```

html

```html
<!DOCTYPE HTML>
<html>
<head>
<meta http-equiv="Content-Type" content="text/html; charset=utf-8"/>
<script type="text/javascript">
//WEB页主线程
var worker =new Worker("worker.js"); //创建一个Worker对象并向它传递将在新线程中执行的脚本的URL
worker.postMessage("hello world");     //向worker发送数据
worker.onmessage =function(evt){     //接收worker传过来的数据函数
   console.log(evt.data);              //输出worker发送来的数据
}
</script>
</head>
<body></body>
</html>
```

**九、Web Storage**

WebStorage是HTML新增的本地存储解决方案之一，但并不是取代cookie而指定的标准，cookie作为HTTP协议的一部分用来处理客户端和服务器的通信是不可或缺的，session正式依赖与实现的客户端状态保持。WebSorage的意图在于解决本来不应该cookie做，却不得不用cookie的本地存储。

websorage拥有5M的存储容量，而cookie却只有4K，这是完全不能比的。

客户端存储数据有两个对象，其用法基本是一致。

localStorage：没有时间限制的数据存储

sessionStorage:在浏览器关闭的时候就会清除。

```css
localStorage.setItem(key,value);//保存数据
    let value = localStorage.getItem(key);//读取数据
    localStorage.removeItem(key);//删除单个数据
    localStorage.clear();//删除所有数据
    let key = localStorage.key(index);//得到某个索引的值
```

**十、WebSocket**

WebSocket协议为web应用程序客户端和服务端之间提供了一种全双工通信机制。

特点：

（1）握手阶段采用HTTP协议，默认端口是80和443

（2）建立在TCP协议基础之上，和http协议同属于应用层

（3）可以发送文本，也可以发送二进制数据。

（4）没有同源限制，客户端可以与任意服务器通信。

（5）协议标识符是ws（如果加密，为wss），如ws://localhost:8023

### 21.结构伪类选择器

##### nth-child系列

```css
:first-child            选择属于父元素的第一个子元素
:last-child             选择属于其父元素最后一个子元素
:nth-child (n)          选择属于其父元素的第n个子元素
:nth-last-child (n)     同上，从最后一个子元素开始计数。
```

1） “n”是自然数 不为0

2） 关键词(odd、even偶数)

3） “n”也可以是表达式 an + b

-n 表示反向， b 表示第几个

```css
例如：

nth-child (-4n+20 )     第20 、16 、12 、8 、4
即前20个，从第20个开始数    20 、20-4、 20-2*4  、
20-3*4  、20-4*4  
```

**注意：** 表达式中的n要放在前面写

​ nth-child的选择器是先排位置，然后再找标签，如果标签和位置对不上，那么这个选择器就是错误的。如下代码

```css
<style>
    div p:nth-child(2){
        /*这是错误的选择器，因为第二个位置的标签是h1*/
        color: pink;
    }
</style>

<div>
    <p>p1</p>
    <h1>h标签</h1>
    <p>p2</p>
</div>
```

##### nth-of-type系列

使用规则与nth-child一样，唯一的区别是，这个伪类选择器的位置，是先把元素找到后，再从上往下排位置

|选择器|例子|例子描述|
|---|---|---|
|:first-of-type|p:first-of-type|选择属于其父元素的首个<br><br>元素的每个<br><br>元素。|
|:last-of-type|p:last-of-type|选择属于其父元素的最后<br><br>元素的每个<br><br>元素。|
|:nth-of-type(_n_)|p:nth-of-type(2)|选择属于其父元素第二个<br><br>元素的每个<br><br>元素。|
|:nth-last-of-type(_n_)|p:nth-last-of-type(2)|同上，但是从最后一个子元素开始计数。|

```css
<style>
    div p:nth-of-type(2){
        /*p2这个文字变成粉色了*/
        color: pink;
    }
</style>

<div>
    <p>p1</p>
    <h1>h标签</h1>
    <p>p2</p>
</div>
```

### 22.盒子布局相关

##### 盒子内减模式

_box-sizing: border-box;_

标准盒子模型是：

border + padding + content 得到实际宽高，实际宽高随着三个值的改变而改变。

ie盒子模型是：

border + padding + content 得到实际宽高，但是不同的是给盒子设置了宽度后，实现宽高就固定了，content会随着三个值的改变而改变

w3c标准盒子模型更多使用于pc端的页面。ie盒子模型更多使用于移动端的页面。改变盒子模型的方法就是修改box-sizing;

##### 计算盒子宽度 – calc 函数

括号里面可以使用 + - * / 来进行计算

```
width: calc(100% - 80px);
```

**注意！ 符号左右要加空格。**

##### 双飞翼布局

（左右两侧宽度固定，中间内容随着页面缩放）

双飞翼布局的实现  
1.eft、center、right三种都设置左浮动

2. 设置center宽度为100%
3. left、right设置margin-left，让左靠左，右靠右，此时left、right遮挡了center区域

```html

<!DOCTYPE html>
<html>
 
<head>
  <meta charset="utf-8">
  <script src="http://lib.sinaapp.com/js/jquery/2.0.2/jquery-2.0.2.min.js"></script>
</head>
<style>
  body {
    min-width: 550px;
    font-weight: bold;
    font-size: 20px;
  }
  #header,
  #footer {
    background: rgba(29, 27, 27, 0.726);
    text-align: center;
    height: 60px;
    line-height: 60px;
  }
  #container {
    overflow: hidden;
  }
  .column {
    text-align: center;
    height: 300px;
    line-height: 300px;
  }
  #left, #right, #center {
    float: left;
  }
  #center {
    width: 100%;
    background: rgb(206, 201, 201);
  }
  #left {
    width: 200px;
    margin-left: -100%;
    background: rgba(95, 179, 235, 0.972);
  }
  #right {
    width: 150px;
    margin-left: -150px;
    background: rgb(231, 105, 2);
  }
  .content {
    margin: 0 150px 0 200px;
  }
</style>
 
<body>
  <div id="header">#header</div>
 
  <div id="container">
    <div id="center" class="column">
      <div class="content">#center</div>
    </div>
    <div id="left" class="column">#left</div>
    <div id="right" class="column">#right</div>
  </div>
 
  <div id="footer">#footer</div>
</body>
 
</html>


```

### 23、背景

##### 1 背景大小（尺寸）

1） background-size:水平 垂直

注意：垂直的可以省略，如果垂直缩放省略的它会根据水平进行等比例缩放。

background-size: 500px 500px;

-webkit-background-size: 500px 500px;

-webkit-这个是我们谷歌和苹果浏览器的兼容性前缀（加上这个

-webkit-就能保证谷歌和苹果浏览下面显示正常）

2）background-size:cover

它是根据父盒子的大小进行等比例缩放，不管是宽度还是高度都必须铺满整个盒子才停止缩放，会溢出父盒子。

3）background-size:contain

总结：它也会进行图片的等比例缩放，但是只要有一个值（不管是宽度还是高度跟父盒子一样了）就停止缩放。

它的好处就能看到完整的图片。

##### 2 背景图片定位区域（源）

background-origin: padding-box 相对于内边距框定位。

​ border-box 相对于边框盒来定位。

​ content-box; 相对于内容框来定位。

##### 3 背景裁减区域

```css
background-clip: border-box|padding-box|content-box;
```

|值|描述|点击[测试](https://www.w3school.com.cn/tiy/c.asp?f=css_background-clip&p=2)|
|:--|:--|:--|
|border-box|背景被裁剪到边框盒。||
|padding-box|背景被裁剪到内边距框。||
|content-box|背景被裁剪到内容框。||

##### 4 多重背景

我们背景图后面还可以在跟一个背景。

background: url(ldh.jpg) no-repeat,url(site-logo.png) repeat-x right bottom;

**注意：**多背景图的一个展示关系是： 先引入的背景图会压住后引入的背景图

##### 5. 背景渐变（颜色渐变）

##### 

总结：从一个边过渡到到另外一个边。

格式background:linear-gradient(起始位置,开始的颜色,结束的颜色)

总结：如果想兼容其他浏览器尽量在

background:-webkit-linear-gradient(起始位置,开始的颜色,结束的颜色)

background:-moz-linear-gradient(起始位置,开始的颜色,结束的颜色)

我们渐变还可以加多个

格式background:linear-gradient(起始位置,第一个颜色 0%,第二个颜色 50%，第三个颜色 100%…);

[线性渐变](https://www.w3school.com.cn/css/css3_gradients.asp)

语法：

```css
background-image: linear-gradient(direction, color-stop1, color-stop2, ...);
```

```css
#box {
  background-image: linear-gradient(red, yellow);
}
```

[径向渐变](https://www.w3school.com.cn/css/css3_gradients_radial.asp)

格式background: radial-gradient(起始位置,开始的颜色,结束的颜色)

语法：

```css
background-image: radial-gradient(shape size at position, start-color, ..., last-color);

shape 参数定义了形状。它可以是值 circle 或 ellipse。其中，circle 表示圆形，ellipse 表示椭圆形。默认值是 ellipse。
```

```css
#box {
  background-image: radial-gradient(red, yellow, green);
}
```

注意: 渐变相当于设置的是背景图

### 24、边框图片

例如：background:url(xx.jpg) 27px no-repeat;指的是图片(url(xx.jpg))，位置(27px)，重复性(no-repeat)。

border-image与此类似，border-image包括图片，剪裁位置（与background位置一样，也是数值，也支持百分值），重复性。  
例如：border-image:url(border.png) 27 repeat; 指的就是图片(url(border.png))，剪裁位置(27)，重复方式(repeat)。

语法：

border-image:source slice repeat;

|值|描述|
|:--|:--|
|_border-image-source_|用在边框的图片的路径。|
|_border-image-slice_|图片边框向内偏移。|
|_border-image-width_|图片边框的宽度。|
|_border-image-outset_|边框图像区域超出边框的量。|
|_border-image-repeat_|图像边框是否应平铺(repeated)、铺满(rounded)或拉伸(stretched)。|

source:所用图像的url地址；  
slice:1~4个长度值（或者百分比），用于设置图片在每一条边上的距离（区域）；  
还是遵循上右下左，顺时针原则,例如值为 30% 35% 40% 30%

repeat：1~2个关键字，用于设置图片在水平方向和竖直方向的重复方式。取值有以下四种：  
stretch：默认值，将图片进行拉伸以填充边框的长  
repeat：沿边框长平铺图片  
round：沿着边框的长整数次的平铺图片（元素可能被自动调整大小以适应该要求）  
space：沿着边框的长整数次的平铺图片（如果图片不能填满元素，则使用空白填充）

案例：

[案例](https://www.w3school.com.cn/tiy/t.asp?f=eg_css3_border-image)

```css
border-image:url(/i/border.png) 30 30 round;
```

```css
border-image:url(/i/border.png) 30 30 stretch;
```

### 25. 过渡 transition

##### 1 体验

如想要看到div的宽度由1000px变为100px的过程 将鼠标移入div 试试

```css
    div {
      width: 1000px;
      height: 100px;
      background-color: aqua;
      /* 要过渡的属性 width*/
      transition-property: width;
      /* 过渡的持续时间 3s*/
      transition-duration: 3s;
    }

    div:hover{
      width: 100px;
    }
```

##### 2 语法

1. `transition-property` 要执行过渡的属性名
    
    如width，height `transition-property: width;` 写`all`代表全部
    
2. `transition-duration` 执行过渡的持续的时间
    
    设置过渡的持续时间 如 `transition-duration:10s`
    
3. `transition-timing-function` 速度曲线 (可省略)
    
    设置变化的速度曲线 如匀速等
    
    - linear： 匀速
        
    - ease： 慢-快-慢 默认值
        
    - ease-in： 慢-快。
        
    - ease-out： 快-慢。
        
    - ease-in-out： 慢-快-慢。
        
    - 贝塞尔曲线（了解）
        
    - steps 设置 跳跃性的动画 （了解）
        
        steps (n) 过渡分成n段
        
        steps (n,start) 在该段时间的开始 触发
        
        steps(n,end) 在该段时间的 末端 出发
        
4. `transition-delay` 延迟时间 （可省略）
    
    设置产生过渡时的延迟时间 如 `transition-delay: 10s;`
    

##### 3 复合写法

可以使用复合写法

```css
 /* 过渡的属性为width 持续3s 匀速 延迟0s */
   transition: width 3s linear 0s;
```

##### 4 多个过渡写法

可以同时对一个元素的多个属性添加过渡 对宽度和高度设置不同的过渡

```css
  transition: 
        width 1s ease-in 1s,
        height 10s ease-in-out 2s;
```

### 26. 2D转换（变换）transform

2d转换是改变标签在**2维平面**上的**位置和形状**的一种技术，先来学习2维坐标系

##### 2维坐标系

**2维坐标系**其实就是指布局的时候的坐标系 如图

##### 2d移动 translate

2d移动是2d转换里面的一种功能，可以改变元素在页面中的位置，类似 **定位**

使用2d移动的步骤：

1. 给元素添加 **转换属性** `transform`
2. 属性值为 `translate(x,y)` 如 `transform:translate(50px,50px)`;

```css
  div{
    transform: translate(50px,50px);
  }
```

**小结**

1. **translate**中的百分比单位是相对于自身元素的 `translate:(50%,50%);`
2. **translate**类似定位，不会影响到其他元素的位置
3. 对行内标签没有效果

##### 2d旋转 rotate

2d旋转指的是让元素在2维平面内顺时针旋转或者逆时针旋转

使用步骤：

1. 给元素添加转换属性 `transform`
2. 属性值为 `rotate(角度)` 如 `transform:rotate(30deg)` 顺时针方向旋转**30度**

```css
div{
      transform: rotate(0deg);
}
```

在浏览器中手动修改 **rotate**

观察过后，2d旋转有以下特点

1. 角度为正时 顺时针 负时 为逆时针
2. 默认旋转的中心点是元素的中心点

##### 转换中心 transform-origin 了解

该属性可以修改元素旋转的时候的中心点

1. transform-origin:**50% 50%;** 默认值 元素的中心位置 百分比是相对于自身的宽度和高度
2. transform-origin:**top left;** 左上角 和 transform-origin：0 0;相同
3. transform-origin:**50px 50px;** 距离左上角 50px 50px 的位置
4. transform-origin：**0**; 只写一个值的时候 第二个值默认为 50%;

##### 2d缩放 scale

缩放，顾名思义，可以放大和缩小。 只要给元素添加上了这个属性就能控制它放大还是缩小

步骤：

1. 给元素添加转换属性 `transform`
2. 转换的属性值为 `scale(宽的倍数,高的倍数)` 如 宽变为两倍，高变为3倍 `transform:scale(2,3)`

```css
div{
    transform:scale(2,3);
}
```

[外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传(img-PPdTRPWT-1646389446731)(F:/叩丁狼/1.html+css/day10-html5+css3/01-课堂笔记-html5+css3两天/assets/1524966701225.png)]

**小结**

1. transform:scale(1,1) 放大一倍 相对于没有放大
2. transform:scale(2,2) 宽和高都放大了2倍
3. transform:scale(2) 只写一个参数 第二个参数则和第一个参数一样 相当于 scale(2,2)
4. transform:scale(0.5,0.5) 缩小
5. transform:scale(-2,-2) 反向放大2倍 很少用负数 容易让人产生误解

### 27. 3D转换（变换）

3d转换是改变标签在3**坐标系**上的**位置和形状**的一种技术 以下知识点最好结合 [3d模型工具来理解](%E6%A1%88%E4%BE%8B/01-%E7%AB%8B%E6%96%B9%E4%BD%93%E6%BC%94%E7%A4%BA.html)

##### 3维坐标系

3维坐标系其实就是指立体空间，立体空间是由3个轴共同组成的

- x轴 **水平向右**
- y轴 **垂直向下**
- z轴 垂直屏幕 由屏幕里面指向屏幕的外面

##### 3d移动 translate3d

**语法：**

1. transform:**translate3d**(x,y,z) 其中 **x y z** 分别指要移动的轴的方向的距离
2. translform:**translateX**(100px) 仅仅是移动在x轴上移动
3. translform:**translateY**(100px) 仅仅是移动在Y轴上移动
4. translform:**translateZ**(100px) 仅仅是移动在Z轴上移动

**注意**:

因为z轴是垂直屏幕，由里指向外面，所以 默认是看不到元素在z轴的方向上移动，想要看到，可以使用下面的 **视距** 属性设置

##### 视距 perspective

1. 设置物体 在z轴上的移动 `translateZ` 一般大于 0 如 `transform:translateZ(100px)`
2. 设置 人和物体的距离 - 视距 这个值规定要设置给**物体的父元素** `perspertive:1000px`
3. 动态改变物体的 `translateZ` 即可观察效果

```css
    /* 父元素 */
    body {
      /* 视距 */
      perspective: 1000px;
    }

    /* 目标 */
    div {
      width: 200px;
      height: 200px;
      background-color: aqua;
      margin: 100px auto;
      /* z轴的移动 */
      transform: translateZ(0px);
    }
```

##### 3d旋转 rotate3d

3d旋转指可以让元素在3维平面内沿着 **x轴，y轴，z轴或者自定义轴**进行旋转

我现在想让元素沿着 x轴正方向旋转90度

```css
    /* 沿着x轴正方向旋转90度 deg为单位 */
      transform: rotateX(90deg);
```

语法

1. `transform:rotateX(45deg);` 沿着x轴正方向旋转 45度
2. `transform:rotateY(45deg)` 沿着y轴正方向旋转 45deg
3. `transform:rotateZ(45deg)` 沿着Z轴正方向旋转 45deg
4. `transform:rotate3d(x,y,z,deg)` 沿着自定义轴旋转 deg为角度 了解即可

##### 3d缩放 scale3d 了解

3d缩放 可以控制元素 在 x轴，y轴，z轴上的缩放，也可以理解为 宽，高，厚度的缩放。 结合[3d模型工具学习](3d%E6%BC%94%E7%A4%BA%E5%B7%A5%E5%85%B7.html)

语法

1. transform: scale3d(1,1,2); 宽，高 缩放一倍，厚度放大两倍
2. `transform: scaleX(1)` 只缩放宽
3. `transform: scaleY(1)` 只缩放高
4. `transform: scaleZ(1)` 只缩放厚

##### 视距原点 perspective-origin

回顾**视距**知识点，

视距可以设置 **人 和 物体** 之间的距离 也就是z轴方向的距离

而 **视距原点** 可以设置 人 站在x轴和y轴的位置

1. 视距原点和视距一样，也是设置给要观察元素的**父元素**上
2. perspective-origin:center center; 默认值是**元素的中心点**
3. perspective-origin:10px； 指定了一个参数的时候，第二个参数默认为center 也就是50%；
4. perspective-origin:10% %； 百分比都是相对于自身的宽度和高度

##### 开启3维立体环境

- `transform-style: preserve-3d;` 开启3维立体环境

##### 3D转换注意点

1. 百分比单位都是相对于自身
2. 视距、视距原点、转换样式 这三个属性都是给**父元素**添加的

### 28. 动画 animation

初学者容易对 **动画** 和 **过渡** 傻傻分不清楚

过渡 只能看到一次变化过程 如 **宽度 1000px 变化到 100px**

**动画 可以设置变化的次数 甚至是无数次**

1. **步骤**
    
2. 在css中定义动画函数
    
3. 给目标元素调用动画函数
    

```css
    /* 1 定义动画函数 */

    @keyframes ani_div {
      0%{
        width: 100px;
        background-color: red;
      }
      50%{
        width: 150px;
        background-color: green;
      }
      100%{
        width: 300px;
        height: 300px;
        background-color: yellow;
      }
    }

    div {
      width: 200px;
      height: 200px;
      background-color: aqua;
      margin: 100px auto;
      /* 2 调用动画 */
      animation-name: ani_div;
      /* 持续时间 */
      animation-duration: 2s;
    }
```

2. **语法**

- animation-name: xxx; 定义动画名（必须）
- animation-duration: 3s; 动画持续时间 （必须）
- animation-timing-function: linear; 设置动画过渡的速度曲线（匀速）
- animation-delay: 0s; 动画延迟时间
- animation-iteration-count: infinite; 循环次数 （无限循环）
- animation-direction：normal 默认 | reverse 反向； 循环方向
- animation-fill-mode：forward； 设置动画结束后的状态停留在100%
- animation-play-state： 控制 running 播放 还是 paused暂停

3. **复合写法**

```css
animation: name duration timing-function delay iteration-count direction fill-mode;
```

多个动画写法 ： 两个动画之间用 **逗号** 分隔

### 29.响应式布局：

CSS 响应式布局也称自适应布局，是 Ethan Marcotte 在 2010 年 5 月份提出的一个概念，简单来讲就是一个网站能够兼容多个不同的终端（设备），而不是为每个终端做一个特定的版本。这个概念是为解决移动端浏览网页而诞生的。  
有几种方式可以实现：

1. 媒体查询
2. 通过js控制（消耗性能）
3. 使用第三方插件（比如bootstrap）

这里以媒体查询为例来具体演示一下响应式布局的实现。  
设置 meta 标签  
首先，我们需要设置 meta 标签来告诉浏览器，让视口（网页的可视区域）的宽度等于设备的宽度，并禁止用户对页面的缩放，如下所示：

```html
<meta name="viewport" content="width=device-width, initial-scale=1, maximum-scale=1, user-scalable=no">
```

然后通过当前屏幕分辨率改变CSS样式 （**媒体查询**）  
@media screen and ( 设置宽高条件 ) { }

```css

        @media screen and (max-width: 640px) {
            body {
                background-color: red;
            }
        }

        /* 假定：640~980 为 ipad的尺寸范围 */
        @media screen and (min-width:641px) and (max-width:980px) {
            body {
                background-color: green;
            }
        }

        /* 假定 大于980 为pc端尺寸范围 */
        @media screen and (min-width:980px) {
            body {
                background-color: blue;
            }
        }
```

**横屏与竖屏**

(orientation:landscape) 横屏

(orientation:portrait) 竖屏

```css
  @media screen and (orientation:landscape) {
      /*当屏幕是横屏时（宽度大于高度就是横屏），执行{}里面的样式代码*/
    body {
        background-color: #000;
      }
```

媒体类型匹配：

- all 匹配所有的媒体类型 默认值 @media all and || @media
    
- screen 匹配 计算机显示器 @media screen and
    
- print 匹配打印机设备 @media print and
    
    媒体关键字【了解】
    
    - not 取反
    - only 实现更好的兼容（使用较多）
    - and 连接（使用较多）
    - or 或者 (使用`，`表示)
    
    ```css
     /* 取反 屏幕宽度不为800px的时候 被选中 */
        @media not screen and (width:800px){
          body{
            background-color: red;
          }
        }
     /* only 更好的兼容 屏幕为800px的时候被选中 */
        @media only screen and (width:800px){
          body{
            background-color: red;
          }
        }
    
      /* or 代码中体现为 逗号(,)  意思屏幕为800px或者600px的时候被选中 */
        @media screen and (width:800px),screen and (width:600px) {
          body{
            background-color: green;
          }
        }
    ```
    
    媒体查询引入方式【掌握】
    
    - **style标签里**或者css文件中
        
        ```html
        <!-- 在style标签里或者在css文件里写媒体查询  -->  
        <style>
            @media screen and (width:800px) {
              body {
                background-color: red;
              }
            }
        </style>
        ```
        
    - **style标签上**
        
        ```html
         <!-- 在style标签上通过属性的方式写媒体查询 -->
        <style media="screen and (width:800px)">
            body {
              background-color: red;
            }
          </style>
        ```
        
    - **link标签上**
        
    
    ```html
     <!--在link标签写媒体查询，根据不同的窗口大小，执行不同的css文件 -->
      <link rel="stylesheet" media="screen and (width:800px)"  href="./base.css">
    ```
    
    ### 
    

### 30.百分比布局：

又叫流式布局，也称为非固定像素布局

​ 原理 通过盒子的宽度设置成百分比来根据屏幕的宽度来进行伸缩，不受固定像素的限制，内容向两侧填充。

流式布局方式是**移动web开发**使用的比较常见的布局方式之一。

​ 数值单位 %

​ 几个百分比布局中常见的属性

- min-width 设置元素的最小宽度, 如果元素的宽度比这个值小，强制按照这个值显示
    
- min-height 设置元素的最小高度
    
- max-width 设置元素的最大宽度, 如果元素的宽度比这个值还大，强制按照这个值显示
    
- max-height 设置元素的最大高度
    

### 31.less

​ 是一门 CSS扩展语言，称为css的预处理器

使用 ：下载 Less 插件 **Easy LESS**

**Easy LESS **插件用来把less文件编译为css文件

安装完毕插件，重新加载下 vscode。

只要保存一下Less文件，会自动生成CSS文件。

###### less插件配置扩展

```js
 "less.compile": {
        "out": "../css/",
        "sourceMap": true
    }

out 配置less自动生成的css文件放在哪个目录下
sourceMap  配置映射文件（可以在浏览器调试bug的时候看到代码在对应的less文件的哪一行）
```

#### less基本语法

##### less变量

变量是指没有固定的值，可以改变的。因为我们CSS中的一些颜色和数值等经常使用。

```less
//变量的定义  @变量名:值;
@base-color: pink;

div{
  width: 100%;
  height: 40px;
  background-color: @base-color;
}
button{
  width: 60px;
  height: 30px;
  background-color: @base-color;
}

```

- 必须有@为前缀
- 不能包含特殊字符
- 不能以数字开头
- 大小写敏感

##### less嵌套

```less
// css写法
#header .logo {
  width: 300px;
}
// 将css改为less
#header {
    .logo {
       width: 300px;
    }
}

```

```less
// css写法
a:hover{
    color:red;
}
// less写法
// 如果遇见 （交集|伪类|伪元素选择器） ，利用&进行连接
a{
  &:hover{
      color:red;
  }
}
```

##### less运算

任何数字、颜色或者变量都可以参与运算。就是Less提供了加（+）、减（-）、乘（*）、除（/）算术运算。

```less
@w:300px;
@color1:green;
@color2:red;

//制作一个高永远是宽度一半的盒子
div{
  //width: @w - 100;//可以
  //width: @w - 200px ;//可以
  width: @w;
  height: @w/2;
  //background-color: @color1 + @color2;  //可以
  //background-color: @color1 + 15; // 可以
  //background-color: @color1 + yellow; // 不可以
}
```

- 乘号（*）和除号（/）的写法
    
- 运算符中间左右有个空格隔开 1px + 5
    
- 对于两个不同的单位的值之间的运算，运算结果的值取第一个值的单位
    
- 如果两个值之间只有一个值有单位，则运算结果就取该单位
    

##### ~“” less编译的转义符

转义在 Less 中用的并不是很多，只有当代码不能被识别时，才需要使用转义，任何 `~"text"` 被编译成 CSS 代码后，都将显示为 `text`。

```less
~""  不想被less解析东西可以放在~"" 当中
.box{
    //（现在less插件升级了，背景的斜杠它认识）
    // 背景连写中，背景位置与背景大小要用/隔开  
	backgound: url(1.png) top right ~"/" 200px 200px;	
}
```

### 32. 字体图标

1. 阿里iconfont 字体图标

​ 链接：http://www.iconfont.cn/

###### 账号

​ 阿里iconfont字体图标的下载需要有自己的一个账号，可以使用阿里员工号（如果你是）或[github](https://github.com/login)号、[微博](https://weibo.com/signup/signup.php)号

###### 登录iconfont

​

###### 图标下载

- 搜索或选择图标
    
- 选中图标，加入购物车
    
- 点击购物车，把图标添加到项目中
    
    点击加号新建项目名，建好名字点击确定，下载添加至项目
    
- 下载图标文件
    
    在我发起的项目里找到对应文件，点击下载至本地
    

###### iconfont的使用-本地【掌握】

​ 阿里妈妈图标库的使用方式有三种，三种方式都能展示字体图标，各有各的优势，使用的步骤也大同小异，这里先给大家介绍其中的一种–`Font class`的方式。

​ **如何查看阿里iconfont字体的三种使用方式的步骤？？**

​

​ **使用Font class方式 展示图标的步骤**

1. 解压下载的文件，把字体图标的相关文件拷贝到自己建好的fonts文件夹中（行业常规习惯）
    
2. 在页面中引入fonts文件夹中的iconfont.css 文件
    
    ```html
    <link rel="stylesheet" href="./fonts/iconfont.css">
    ```
    
3. 在下载的字体文件中的demo_index.html中挑选相应的图标，  
    拷贝他的类名，设置到页面展示图标的标签上 （第一个类名要写 iconfont，然后再追加拷贝的类名） （注意前面没有点）
    

###### iconfont的使用-线上【掌握】

1. 在自己的字体图标项目库中，点击查看在线链接 ，复制在线的字体图标链接地址
    
2. 后面的步骤与本地的一模一样
    
    ```html
    <html>
    <head>
            ...
            <!-- 本地的方式 -->
            <!-- <link rel="stylesheet" href="./fonts/iconfont.css"> -->
            <!-- 使用线上的地址，在复制的地址前面加上http: -->
        <link rel="stylesheet" href="http://at.alicdn.com/t/font_2170259_hm4u8yi7liu.css">
    </head>
    
    <body>
         <div class="iconfont icon-camera"></div>
    </body>
    </html>
    ```
    

###### 其他一些字体图标

- **icommon字体图标** http://www.iconfont.cn/
    
- **Font-Awesome** [http://fortawesome.github.io/Font-Awesome/](http://fortawesome.github.io/Font-Awesome/)
    
- …
    

### 33.理想视口

开发会用理想视口，而理想视口就是将布局视口的宽度修改为视觉视口

最标准的viewport设置

- 视口宽度和设备保持一致
    
- 视口的默认缩放比例1.0
    
- 最大允许的缩放比例1.0
    
- 最小允许的缩放比例1.0
    
- 不允许用户自行缩放
    

##### meta标签

```html
<meta name="viewport"
        content="width=device-width, initial-scale=1.0,maximum-scale=1,minimum-scale=1,user-scalable=no">
```

### 34.移动端

浏览器兼容问题

浏览器前缀

```
Chrome(谷歌浏览器) ：WebKit内核     -webkit-
Safari(苹果浏览器) ：WebKit内核        -webkit-
Firefox(火狐浏览器) ：Gecko内核         -moz-
IE(IE浏览器) ：          Trident内核        -ms-
Opera(欧朋浏览器) ：Presto内核          -o-
```

​ 移动端浏览器基本以 webkit 内核为主，因此我们就考虑webkit兼容性问题。

​ 我们可以放心使用 H5 标签和 CSS3 样式。

​ 同时我们浏览器的私有前缀我们只需要考虑添加 webkit 即可

##### 移动端公共样式 reset.css

```css
@charset "utf-8";
/* 禁用iPhone中Safari的字号自动调整 */
html {
    -webkit-text-size-adjust: 100%;
    -ms-text-size-adjust: 100%;
}
/* 去除iPhone中默认的input样式 */
input[type="submit"], input[type="reset"], input[type="button"]{ -webkit-appearance:none; resize: none; }
/* 取消链接高亮  */
body,div,ul,li,ol,h1,h2,h3,h4,h5,h6,input,textarea,select,p,dl,dt,dd,a,img,button,form,table,th,tr,td,tbody,article,aside, details,figcaption,figure,footer,header,hgroup, menu,nav,section{ -webkit-tap-highlight-color:rgba(0, 0, 0, 0); }
/* 设置HTML5元素为块 */
article, aside, details,figcaption,figure,footer,header,hgroup, menu,nav,section { display: block; }
/* 图片自适应 */
img { vertical-align: middle; max-width: 100%; height: auto; border:none; }
/* 初始化 */
body,ul,li,ol,h1,h2,h3,h4,h5,h6,input,textarea,select,p,dl,dt,dd,a,img,button,form,table,th,tr,td,tbody,article, 
aside,details,figcaption,figure,footer,header,hgroup,menu,nav,section{ margin:0; padding:0; border: 0 none; }
body{
	/*强制隐藏横向滚动条*/
    overflow-x: hidden; 
    background-color: #f5f5f5;
}
em,i{ font-style:normal; }
strong,b{ font-weight: normal; }
a{ text-decoration:none; color:#333; }
li{ list-style:none; }
h1, h2, h3, h4, h5, h6{ font-size:100%; font-weight: normal; }
input{ outline-style:none; }
```

移动端特殊样式

```
    /*CSS3盒子模型*/
    box-sizing: border-box;
    -webkit-box-sizing: border-box;
    /*点击高亮我们需要清除清除  设置为transparent 完成透明*/
    -webkit-tap-highlight-color: transparent;
    /*在移动端浏览器默认的外观在iOS上加上这个属性才能给按钮和输入框自定义样式*/
    -webkit-appearance: none;
    /*禁用长按页面时的弹出菜单*/
    img,a { -webkit-touch-callout: none; }

```

##### 移动端常见布局

- flex 弹性布局（强烈推荐）
    
- vw vh 布局
    
- rem+媒体查询布局
    
- 混合布局（前面几种布局都会使用到，也是开发中常见的使用）
    

### 34.弹性布局

##### 弹性布局又叫flex布局

1. 开启弹性布局：display: flex;
    
2. 设置属性
    
    1. flex-direction – 设置 主轴方向
        
        - row - 横向为主轴 X （默认）
        - column - 纵向为主轴 Y
    2. justify-content – 设置主轴对齐方式
        
        - justify-content: flex-start; – 位于容器的开头
        - justify-content: flex-end; – 位于容器的末尾
        - justify-content: center; – 水平居中(常用)
        - justify-content: space-between; – 两边贴边，中间留空 (常用)
        - justify-content: space-around; – 平分剩余空间
    3. align-items – 设置侧轴对齐方式
        
        - align-items: stretchl; – 默认值，拉伸填满
        - align-items: center; – 设置垂直据中(常用)
        - align-items: flex-start; – – 位于容器的开头
        - align-items: flex-end; – 位于容器的末尾
        - align-items: baselinel; – 位于容器基线上
    4. align-content – 设置多行时的对齐方式
        
        - align-content: stretch; – 默认值，拉伸自适应
            
        - align-content: flex-start; – 位于容器的开头
            
        - align-content: flex-end; – 位于容器的末尾
            
        - align-content: center; – 水平垂直居中 (常用)
            
        - align-content: space-between; – 两边贴边，中间留空 (常用)
            
        - align-content: space-around; – 平分剩余空间
            
    5. flex-wrap – 设置是否换行
        
        - nowrap – 不换行
        - wrap – 换行
    6. order: num; – 设置排列顺序，默认为 0
        
    7. align-self – 设置元素自身，在侧轴上的对齐方式。脱离原来的排序限制。
        
    8. flex: num; – 设置子元素占用空间份数
        

##### rem布局

用 rem 布局时，使用 vscode中的 px to rem插件进行转换

1. 假设把750的设计稿划分为**10**等份  
    那么 1个格子 = 750/10 = 75px
    
2. 所以我们要在750的屏幕使用rem单位等比例还原设计稿的时，也要使用等比例切割，把页面划分为10等分
    
    即给html设置font-size值为：75px；
    
    即 1rem = 75px； ====> 1px = 1/75rem =0.0133rem ;
    

扩展设置 -------Root Font Size default：16 改为 75

1rem = 一个根标签 html标签 标准字体的大小 root font-size默认是1rem = 16px

1em = 当前标签的标准字体大小

100vw 就是 当前页面视口的宽度

100vh 就是 当前页面视口的高度

% 相对于父元素。正常情况下是通过属性定义自身或其他元素

px 像素

**下面这段js代码的作用，就是自动获取屏幕的**

```js
var winW = document.documentElement.clientWidth; // 获取屏幕宽度  
var htmlFont = winW/10; // 屏幕宽度/ 10
// 把屏幕宽/10 的结果设置给html的font-size
document.getElementsByTagName('html')[0].style.fontSize = htmlFont+'px';
```

现在，在不同的机型下，html的字体大小就不同，即1个rem所表示的像素就不同。所以把元素的宽度、字体大小等属性单位写成rem，就可以动态设置这些属性。在不同的浏览器分辨率下有最好的展示（按照设计图比例）。

```html
<!DOCTYPE html>
<html lang="en" style="font-size: 75px;">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <style>
        .box1 {
            width: 100px;
            height: 100px;
            background-color: pink;
            font-size: 12px;
        }

        .box2 {
            width: 1.33rem;
            height: 1.33rem;
            background-color: green;
            /* 12*0.0133rem = 0.1596 */
            font-size: 0.1596rem;
        }
    </style>
</head>

<body>
    <div class="box1">
        100px * 100px 的盒子
    </div>
    <div class="box2">
        1.33rem * 1.33rem 的盒子
    </div>
</body>
</html>
<!--下面这段script标签里面的js代码不用大家写，直接复制粘贴到html页面的后面即可-->
<script>
    function setFont() {
        var winW = document.documentElement.clientWidth
        var htmlFont = winW / 10;
        document.getElementsByTagName('html')[0].style.fontSize = htmlFont + 'px';
    }
    setFont();
    window.onresize = function () {
        setFont();
    }
</script>
```

位于容器的末尾  
- justify-content: center; – 水平居中(常用)  
- justify-content: space-between; – 两边贴边，中间留空 (常用)  
- justify-content: space-around; – 平分剩余空间

3. align-items – 设置侧轴对齐方式
    
    - align-items: stretchl; – 默认值，拉伸填满
    - align-items: center; – 设置垂直据中(常用)
    - align-items: flex-start; – – 位于容器的开头
    - align-items: flex-end; – 位于容器的末尾
    - align-items: baselinel; – 位于容器基线上
4. align-content – 设置多行时的对齐方式
    
    - align-content: stretch; – 默认值，拉伸自适应
        
    - align-content: flex-start; – 位于容器的开头
        
    - align-content: flex-end; – 位于容器的末尾
        
    - align-content: center; – 水平垂直居中 (常用)
        
    - align-content: space-between; – 两边贴边，中间留空 (常用)
        
    - align-content: space-around; – 平分剩余空间
        
5. flex-wrap – 设置是否换行
    
    - nowrap – 不换行
    - wrap – 换行
6. order: num; – 设置排列顺序，默认为 0
    
7. align-self – 设置元素自身，在侧轴上的对齐方式。脱离原来的排序限制。
    
8. flex: num; – 设置子元素占用空间份数
    

##### rem布局

用 rem 布局时，使用 vscode中的 px to rem插件进行转换

1. 假设把750的设计稿划分为**10**等份  
    那么 1个格子 = 750/10 = 75px
    
2. 所以我们要在750的屏幕使用rem单位等比例还原设计稿的时，也要使用等比例切割，把页面划分为10等分
    
    即给html设置font-size值为：75px；
    
    即 1rem = 75px； ====> 1px = 1/75rem =0.0133rem ;
    

扩展设置 -------Root Font Size default：16 改为 75

1rem = 一个根标签 html标签 标准字体的大小 root font-size默认是1rem = 16px

1em = 当前标签的标准字体大小

100vw 就是 当前页面视口的宽度

100vh 就是 当前页面视口的高度

% 相对于父元素。正常情况下是通过属性定义自身或其他元素

px 像素

**下面这段js代码的作用，就是自动获取屏幕的**

```js
var winW = document.documentElement.clientWidth; // 获取屏幕宽度  
var htmlFont = winW/10; // 屏幕宽度/ 10
// 把屏幕宽/10 的结果设置给html的font-size
document.getElementsByTagName('html')[0].style.fontSize = htmlFont+'px';
```

现在，在不同的机型下，html的字体大小就不同，即1个rem所表示的像素就不同。所以把元素的宽度、字体大小等属性单位写成rem，就可以动态设置这些属性。在不同的浏览器分辨率下有最好的展示（按照设计图比例）。

```html
<!DOCTYPE html>
<html lang="en" style="font-size: 75px;">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <style>
        .box1 {
            width: 100px;
            height: 100px;
            background-color: pink;
            font-size: 12px;
        }

        .box2 {
            width: 1.33rem;
            height: 1.33rem;
            background-color: green;
            /* 12*0.0133rem = 0.1596 */
            font-size: 0.1596rem;
        }
    </style>
</head>

<body>
    <div class="box1">
        100px * 100px 的盒子
    </div>
    <div class="box2">
        1.33rem * 1.33rem 的盒子
    </div>
</body>
</html>
<!--下面这段script标签里面的js代码不用大家写，直接复制粘贴到html页面的后面即可-->
<script>
    function setFont() {
        var winW = document.documentElement.clientWidth
        var htmlFont = winW / 10;
        document.getElementsByTagName('html')[0].style.fontSize = htmlFont + 'px';
    }
    setFont();
    window.onresize = function () {
        setFont();
    }
</script>
```

如有错误请指正，顺便动动小手点个赞
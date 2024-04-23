[【超用心整理】Markdown常用语法介绍，看这一个就够了_markdown语法-CSDN博客](https://blog.csdn.net/weixin_43863919/article/details/124648510?ops_request_misc=%257B%2522request%255Fid%2522%253A%2522170668453816800184157347%2522%252C%2522scm%2522%253A%252220140713.130102334..%2522%257D&request_id=170668453816800184157347&biz_id=0&utm_medium=distribute.pc_search_result.none-task-blog-2~all~top_click~default-4-124648510-null-null.142^v99^pc_search_result_base4&utm_term=markdown%E8%AF%AD%E6%B3%95&spm=1018.2226.3001.4187)
<h2><a id="Markdown_0"></a>Markdown常用语法介绍</h2><p>Markdown是一种使用一定的语法将普通的文本转换成HTML标签文本的编辑语言&#xff0c;它的特点是可以使用普通的文本编辑器来编写&#xff0c;只需要按照特定的语法标记就可以得到丰富多样的HTML格式的文本。本文就来介绍一些常用的Markdown语法以及推荐几款方便又实用的Markdown编辑器。</p>
<h2><a id="_3"></a>换行问题</h2>
<p>换行是markdown最基本的语法规则&#xff0c;也是它不同于普通文本的地方&#xff0c;想要在某一行之后进行换行只按常规的Enter键是不行的。换行有3种方式&#xff1a;</p>
<ol><li>在行的末尾添加至少两个空格&#xff0c;然后再接Enter另起一行&#xff1b;</li><li>第2种方式是在需要换行的两行内容之间空一行&#xff1b;</li><li>第3种方式是在需要换行的内容末尾添加一个换行标签&#xff0c;也就是<code>&lt;br&gt;</code>标签。</li></ol>
<h2><a id="_9"></a>标题分级</h2>
<p>在当前行之前输入 “#”&#43;&#34;空格&#34;可以使当前行被识别为标题</p>
<blockquote>
<p>&#34;# &#34; -&gt; 一级标题是<br /> &#34;## &#34; -&gt; 二级标题<br /> &#34;### &#34; -&gt; 三级标题</p>
</blockquote>
<h3><a id="_16"></a>标题分级另一种写法</h3>
<p>在当前行的下一行输入一个或者多个&#34;&#61;“和”-&#34;可以使当前行被识别为标题</p>
<blockquote>
<p>“这是一个一级标题”<br /> “&#61;”</p>
<p>“这是一个二级标题”<br /> “-”</p>
</blockquote>
<h2><a id="_24"></a>分割线</h2>
<p>使用三个或以上的 “-” 或者 “*” 表示(混合的不行)&#xff0c;且这一行只有符号&#xff0c;<strong>注意不要被识别为二级标题即可&#xff0c;意思是上面需要是空行</strong>&#xff0c;例如中间或者前面可以加空格。</p>
<blockquote>
<p><strong>语法</strong></p>
</blockquote>
<blockquote>
<p>***<br /> ******<br /> ---<br /> ------</p>
</blockquote>
<h2><a id="_35"></a>斜体和粗体</h2>
<p>使用 (<code>*</code>或者<code>_</code> )和( <code>**</code>或者<code>__</code>) 分别表示斜体和粗体&#xff0c;删除线使用两个 <code>~</code> 表示</p>
<blockquote>
<p><strong>语法</strong></p>
</blockquote>
<blockquote>
<p>*我是斜体*<br /> _我是斜体_<br /> **我是加粗**<br /> __我是加粗__<br /> ~~我是删除~~<br /> ***我是又粗又斜***<br /> ___我是又粗又斜___</p>
</blockquote>
<h2><a id="_48"></a>超链接和图片引用</h2>
<h3><a id="_49"></a>超链接</h3>
<h4><a id="_50"></a>内联超链接</h4>
<p>使用<code>[链接文字](链接地址)</code>来表示&#xff0c;如果要给链接一个提示信息&#xff0c;可以在链接用引号把文字包围起来&#xff0c;就像这样<code>[链接文字](链接地址&#43;空格&#43;&#34;文字说明&#34;)</code></p>
<blockquote>
<p><strong>语法</strong></p>
</blockquote>
<blockquote>
<p>[链接例子《就是外在文字》](http://www.baidu.com/&#34; 我是说明文字&#xff1a;我其实就是HTML 的&lt;a&gt; 标签的 Title 属性&#34;)</p>
</blockquote>
<h4><a id="_56"></a>自动超链接</h4>
<p>以比较简短的自动链接形式来处理网址和电子邮件信箱&#xff0c;只要是用<code>&lt;&gt;</code>包起来&#xff0c; Markdown 就会自动把它转成链接</p>
<blockquote>
<p><strong>语法</strong></p>
</blockquote>
<blockquote>
<p>&lt;http://example.com/&gt;</p>
</blockquote>
<h4><a id="_64"></a>引用式链接</h4>
<p>在任意地方使用<code>[链接引用标记]:链接地址&#43;空格&#43;&#34;文字说明&#34;</code> 来定义引用的链接地址,然后使用<code>[链接文字][链接引用标记]</code>放在需要插入链接的地方</p>
<blockquote>
<p><strong>语法</strong></p>
</blockquote>
<blockquote>
<p>[link1]:http://www.baidu.com/ “baidu.com 其实就是HTML 的&lt;a&gt; 标签的 Title 属性”<br /> [引用式链接例子《就是外在文字》][link1]</p>
</blockquote>
<h5><a id="_71"></a>引用式链接-简化</h5>
<p>该功能让你可以省略指定链接标记&#xff0c;这种情形下&#xff0c;链接标记会视为等同于链接文字&#xff0c;只要在链接文字后面加上一个空的方括号&#xff0c;如果你要让 “Google” 链接到 <a href="[http://google.com/](http://google.com/)" rel="nofollow">google.com</a>,这么写就行</p>
<blockquote>
<p><strong>语法</strong></p>
</blockquote>
<blockquote>
<p>[Google][]<br /> [Google]: http://google.com/</p>
</blockquote>
<h3><a id="_81"></a>图片引用</h3>
<h4><a id="_82"></a>内联式图片引用</h4>
<p>图片引用仅在超链接前多了一个 <code>!</code> &#xff0c;一般是<code>![图片文字](图片地址&#43;空格&#43;&#34;文字说明&#34;)</code></p>
<blockquote>
<p><strong>语法</strong></p>
</blockquote>
<blockquote>
<p>![图片例子《就是Alt属性》](http://www.baidu.com/images/logo.png “我是说明文字&#xff1a;我其实就是HTML 的&lt;a&gt; 标签的 Title 属性”)</p>
</blockquote>
<h4><a id="_88"></a>引用式图片引用</h4>
<p>在任意地方使用<code>[图片引用标记]:图片地址&#43;空格&#43;&#34;文字说明&#34;</code> 来定义引用的图片链接地址,然后使用<code>[图片文字][图片引用标记]</code>放在需要插入图片链接的地方</p>
<blockquote>
<p><strong>语法</strong></p>
</blockquote>
<blockquote>
<p>[link2]:http://www.baidu.com/images/logo.png “baidu.com 其实就是HTML 的&lt;a&gt; 标签的 Title 属性”<br /> ![引用式图片链接例子《就是Alt属性》][link2]</p>
</blockquote>
<h3><a id="_96"></a>带有链接的图片</h3>
<p>部分markdown编辑器只需要将链接代码套在图片代码外边就可以实现。</p>
<blockquote>
<p><strong>语法</strong></p>
</blockquote>
<blockquote>
<p>[![图片例子](http://www.baidu.com/images/logo.png “图片说明文字”)](http://www.baidu.com/ “链接说明文字”)</p>
</blockquote>
<h2><a id="_103"></a>无序列表</h2>
<p>使用 <code>-</code>、<code>&#43;</code> 和 <code>*</code>&#43;<code>空格</code> &#43;<code>文字内容</code> 表示无序列表<br /> 可用<code>tab</code> 或者<code>空格</code> &#43; <code>-</code>、<code>&#43;</code> 或者 <code>*</code> &#43;<code>文字内容</code>使列表嵌套<br /> <strong>成功嵌套的条件是</strong>下一层的<code>-</code>、<code>&#43;</code> 和 <code>*</code> 的前面的空白长度满足以下条件</p>
<pre><code>tab长度×(层数-1) &lt; 空白长度 ≤ tab长度×层数
</code></pre>
<blockquote>
<p> &#43; 第一层<br />    * 第二层<br />     &#43; 第三层</p>
<p> &#43; 再来一个第一层</p>
</blockquote>
<h2><a id="_117"></a>有序列表</h2>
<p>使用 <code>1.</code> &#43;<code>空格</code> &#43;<code>文字内容</code> 表示有序列表&#xff0c;可嵌套。<br /> 可用<code>tab</code> 或者<code>空格</code> &#43; <code>-</code>、<code>&#43;</code> 或者 <code>*</code> &#43;<code>文字内容</code>使列表嵌套<br /> <strong>成功嵌套的条件是</strong>下一层的<code>-</code>、<code>&#43;</code> 和 <code>*</code> 的前面的空白长度满足以下条件</p>
<pre><code>tab长度×(层数-1) &lt; 空白长度 ≤ tab长度×层数
</code></pre>
<blockquote>
<p><strong>语法</strong></p>
</blockquote>
<blockquote>
<p> 1. 第一层<br />    1. 第二层<br />     1. 第三层</p>
<p>  2. 再来一个第一层</p>
</blockquote>
<blockquote>
<p><strong>实例</strong></p>
</blockquote>
<blockquote>
<ol><li>第一层</li><li>第二层.1</li><li>第二层.2
<ol><li>第三层.1</li><li>第三层.2</li></ol> </li><li>第二层.3</li></ol>
<blockquote></blockquote>
<ol><li>在列表结束敲二个空行&#xff0c;在第二个空行中写入任何内容都可以重开一个计数列表</li></ol>
</blockquote>
<h2><a id="_144"></a>文字引用</h2>
<p>使用 <code>&gt;</code> 表示&#xff0c;可以有多个 <code>&gt;</code>&#xff0c;表示层级更深</p>
<p>要从深层到浅层需要在浅层上方留一个有与层数相同个数 <code>&gt;</code>的空行</p>
<blockquote>
<p><strong>语法</strong></p>
</blockquote>
<blockquote>
<p>&gt;文字内容<br /> &gt;文字内容<br /> &gt;&gt;文字内容<br /> &gt;<br /> &gt;文字内容<br /> &gt;文字内容</p>
</blockquote>
<blockquote>
<p><strong>实例</strong></p>
</blockquote>
<blockquote>
<p>文字内容<br /> 文字内容</p>
<blockquote>
<p>文字内容</p>
</blockquote>
<p>文字内容<br /> 文字内容</p>
</blockquote>
<h2><a id="_169"></a>行内代码块</h2>
<p>使用 &#34; &#96; &#34; 把代码包围起来即可</p>
<blockquote>
<p><strong>语法</strong></p>
</blockquote>
<blockquote>
<p>&#96;a &#61; 1&#96;</p>
</blockquote>
<p>如果要在代码区段内插入反引号&#xff0c;你可以用多个反引号来开启和结束代码区段&#xff1a;</p>
<blockquote>
<p><strong>语法</strong><br /> &#96;&#96; There is a literal backtick (&#96;) here.&#96;&#96;</p>
</blockquote>
<h2><a id="_182"></a>代码块</h2>
<h3><a id="_184"></a>方法一</h3>
<p>使用四个空格缩进表示代码块&#xff0c;</p>
<blockquote>
<p><strong>语法</strong></p>
</blockquote>
<blockquote>
<pre><code> import os
print(&#34;hello world&#34;)
def show_time():
return time.time()
</code></pre>
</blockquote>
<h3><a id="_195"></a>方法二</h3>
<p>一些 IDE 支持行数提示和着色&#xff0c;一般使用三个 &#34; &#96; &#34; 表示&#xff0c;例如<br /> 代码块使用3个 &#34; &#96; &#34;包围起来表示&#xff0c;而且代码块的第一行的3个 &#34; &#96; &#34; 后面可以写上代码的编程语言&#xff0c;方便Markdown转化之后进行高亮显示&#xff0c;如写上python或者js</p>
<blockquote>
<p><strong>语法</strong></p>
</blockquote>
<blockquote>
<pre><code>&#96;&#96;&#96;python
import os
print(&#34;hello world&#34;)
def show_time():
return time.time()
&#96;&#96; &#96;
</code></pre>
</blockquote>
<h2><a id="_211"></a>表格</h2>
<p>表格由3个部分组成</p>
<p>第一个部分是表格的标题&#xff0c;使用<code>\</code>来作为列的分割<br /> 第二个部分是表示列的对齐方式&#xff0c;有左对齐、居中对齐和居右对齐三种类型&#xff0c;直接看例子吧&#xff0c; <code>---</code> 表示了默认的<strong>左对齐</strong>&#xff0c; <code>:---</code> 表示 <strong>左对齐</strong> &#xff0c; <code>---:</code> 表示 <strong>右对齐</strong> &#xff0c; <code>:---:</code> 表示<strong>居中对齐</strong><br /> 第三个部分就是内容了&#xff0c;表示方式跟标题一样&#xff0c;可以有多行</p>
<blockquote>
<p><strong>语法</strong></p>
</blockquote>
<blockquote>
<p>\左对齐标题\右对齐标题\居中对齐标题\<br /> \-\------: \:------: \<br /> \居左\居右\居中\<br /> \测试文本\测试文本\测试文本\</p>
</blockquote>
<blockquote>
<p><strong>实例</strong></p>
</blockquote>
<blockquote>
<table><thead><tr><th>左对齐标题</th><th align="right">右对齐标题</th><th align="center">居中对齐标题</th></tr></thead><tbody><tr><td>居左</td><td align="right">居右</td><td align="center">居中</td></tr><tr><td>测试文本</td><td align="right">测试文本</td><td align="center">测试文本</td></tr></tbody></table>
</blockquote>
<h2><a id="_233"></a>流程图</h2>
<p>不同的Markdown解析器原理不同&#xff0c;不一定支持流程图<br /> obsidian 支持 mermaid 流程图。其他的流程图也许要安装插件<br /> mermaid文档: https://mermaid-js.github.io/mermaid/#/README<br /> mermaid在线编辑器: https://mermaid-js.github.io/mermaid-live-editor</p>
<blockquote>
<p><strong>语法</strong></p>
</blockquote>
<blockquote>
<pre><code> &#96;&#96;&#96;mermaid
sequenceDiagram
Alice-&gt;&gt;John: Hello John, how are you?
loop Healthcheck
John-&gt;&gt;John: Fight against hypochondria
end
Note right of John: Rational thoughts!
John--&gt;&gt;Alice: Great!
John-&gt;&gt;Bob: How about you?
Bob--&gt;&gt;John: Jolly good!
&#96;&#96;&#96;
</code></pre>
</blockquote>
<blockquote>
<p><strong>实例</strong></p>
</blockquote>
<blockquote>
<div class="mermaid sequence-diagram">
<svg id="mermaid-svg-qawW8Z3ZG73cWxBa" width="100%" xmlns="http://www.w3.org/2000/svg" height="594" style="max-width: 712px;" viewbox="-50 -10 712 594" >
<style>#mermaid-svg-qawW8Z3ZG73cWxBa {font-family:"trebuchet ms",verdana,arial,sans-serif;font-size:16px;fill:#333;}#mermaid-svg-qawW8Z3ZG73cWxBa .error-icon{fill:#552222;}#mermaid-svg-qawW8Z3ZG73cWxBa .error-text{fill:#552222;stroke:#552222;}#mermaid-svg-qawW8Z3ZG73cWxBa .edge-thickness-normal{stroke-width:2px;}#mermaid-svg-qawW8Z3ZG73cWxBa .edge-thickness-thick{stroke-width:3.5px;}#mermaid-svg-qawW8Z3ZG73cWxBa .edge-pattern-solid{stroke-dasharray:0;}#mermaid-svg-qawW8Z3ZG73cWxBa .edge-pattern-dashed{stroke-dasharray:3;}#mermaid-svg-qawW8Z3ZG73cWxBa .edge-pattern-dotted{stroke-dasharray:2;}#mermaid-svg-qawW8Z3ZG73cWxBa .marker{fill:#333333;stroke:#333333;}#mermaid-svg-qawW8Z3ZG73cWxBa .marker.cross{stroke:#333333;}#mermaid-svg-qawW8Z3ZG73cWxBa svg{font-family:"trebuchet ms",verdana,arial,sans-serif;font-size:16px;}#mermaid-svg-qawW8Z3ZG73cWxBa .actor{stroke:hsl(259.6261682243, 59.7765363128%, 87.9019607843%);fill:#ECECFF;}#mermaid-svg-qawW8Z3ZG73cWxBa text.actor&gt;tspan{fill:black;stroke:none;}#mermaid-svg-qawW8Z3ZG73cWxBa .actor-line{stroke:grey;}#mermaid-svg-qawW8Z3ZG73cWxBa .messageLine0{stroke-width:1.5;stroke-dasharray:none;stroke:#333;}#mermaid-svg-qawW8Z3ZG73cWxBa .messageLine1{stroke-width:1.5;stroke-dasharray:2,2;stroke:#333;}#mermaid-svg-qawW8Z3ZG73cWxBa #arrowhead path{fill:#333;stroke:#333;}#mermaid-svg-qawW8Z3ZG73cWxBa .sequenceNumber{fill:white;}#mermaid-svg-qawW8Z3ZG73cWxBa #sequencenumber{fill:#333;}#mermaid-svg-qawW8Z3ZG73cWxBa #crosshead path{fill:#333;stroke:#333;}#mermaid-svg-qawW8Z3ZG73cWxBa .messageText{fill:#333;stroke:#333;}#mermaid-svg-qawW8Z3ZG73cWxBa .labelBox{stroke:hsl(259.6261682243, 59.7765363128%, 87.9019607843%);fill:#ECECFF;}#mermaid-svg-qawW8Z3ZG73cWxBa .labelText,#mermaid-svg-qawW8Z3ZG73cWxBa .labelText&gt;tspan{fill:black;stroke:none;}#mermaid-svg-qawW8Z3ZG73cWxBa .loopText,#mermaid-svg-qawW8Z3ZG73cWxBa .loopText&gt;tspan{fill:black;stroke:none;}#mermaid-svg-qawW8Z3ZG73cWxBa .loopLine{stroke-width:2px;stroke-dasharray:2,2;stroke:hsl(259.6261682243, 59.7765363128%, 87.9019607843%);fill:hsl(259.6261682243, 59.7765363128%, 87.9019607843%);}#mermaid-svg-qawW8Z3ZG73cWxBa .note{stroke:#aaaa33;fill:#fff5ad;}#mermaid-svg-qawW8Z3ZG73cWxBa .noteText,#mermaid-svg-qawW8Z3ZG73cWxBa .noteText&gt;tspan{fill:black;stroke:none;}#mermaid-svg-qawW8Z3ZG73cWxBa .activation0{fill:#f4f4f4;stroke:#666;}#mermaid-svg-qawW8Z3ZG73cWxBa .activation1{fill:#f4f4f4;stroke:#666;}#mermaid-svg-qawW8Z3ZG73cWxBa .activation2{fill:#f4f4f4;stroke:#666;}#mermaid-svg-qawW8Z3ZG73cWxBa .actorPopupMenu{position:absolute;}#mermaid-svg-qawW8Z3ZG73cWxBa .actorPopupMenuPanel{position:absolute;fill:#ECECFF;box-shadow:0px 8px 16px 0px rgba(0,0,0,0.2);filter:drop-shadow(3px 5px 2px rgb(0 0 0 / 0.4));}#mermaid-svg-qawW8Z3ZG73cWxBa .actor-man line{stroke:hsl(259.6261682243, 59.7765363128%, 87.9019607843%);fill:#ECECFF;}#mermaid-svg-qawW8Z3ZG73cWxBa .actor-man circle,#mermaid-svg-qawW8Z3ZG73cWxBa line{stroke:hsl(259.6261682243, 59.7765363128%, 87.9019607843%);fill:#ECECFF;stroke-width:2px;}#mermaid-svg-qawW8Z3ZG73cWxBa :root{--mermaid-font-family:"trebuchet ms",verdana,arial,sans-serif;}</style>
<g></g>
<defs>
<symbol id="computer" width="24" height="24">
<path transform="scale(.5)" d="M2 2v13h20v-13h-20zm18 11h-16v-9h16v9zm-10.228 6l.466-1h3.524l.467 1h-4.457zm14.228 3h-24l2-6h2.104l-1.33 4h18.45l-1.297-4h2.073l2 6zm-5-10h-14v-7h14v7z"></path>
</symbol>
</defs>
<defs>
<symbol id="database" fill-rule="evenodd">
<path transform="scale(.5)" d="M12.258.001l.256.004.255.005.253.008.251.01.249.012.247.015.246.016.242.019.241.02.239.023.236.024.233.027.231.028.229.031.225.032.223.034.22.036.217.038.214.04.211.041.208.043.205.045.201.046.198.048.194.05.191.051.187.053.183.054.18.056.175.057.172.059.168.06.163.061.16.063.155.064.15.066.074.033.073.033.071.034.07.034.069.035.068.035.067.035.066.035.064.036.064.036.062.036.06.036.06.037.058.037.058.037.055.038.055.038.053.038.052.038.051.039.05.039.048.039.047.039.045.04.044.04.043.04.041.04.04.041.039.041.037.041.036.041.034.041.033.042.032.042.03.042.029.042.027.042.026.043.024.043.023.043.021.043.02.043.018.044.017.043.015.044.013.044.012.044.011.045.009.044.007.045.006.045.004.045.002.045.001.045v17l-.001.045-.002.045-.004.045-.006.045-.007.045-.009.044-.011.045-.012.044-.013.044-.015.044-.017.043-.018.044-.02.043-.021.043-.023.043-.024.043-.026.043-.027.042-.029.042-.03.042-.032.042-.033.042-.034.041-.036.041-.037.041-.039.041-.04.041-.041.04-.043.04-.044.04-.045.04-.047.039-.048.039-.05.039-.051.039-.052.038-.053.038-.055.038-.055.038-.058.037-.058.037-.06.037-.06.036-.062.036-.064.036-.064.036-.066.035-.067.035-.068.035-.069.035-.07.034-.071.034-.073.033-.074.033-.15.066-.155.064-.16.063-.163.061-.168.06-.172.059-.175.057-.18.056-.183.054-.187.053-.191.051-.194.05-.198.048-.201.046-.205.045-.208.043-.211.041-.214.04-.217.038-.22.036-.223.034-.225.032-.229.031-.231.028-.233.027-.236.024-.239.023-.241.02-.242.019-.246.016-.247.015-.249.012-.251.01-.253.008-.255.005-.256.004-.258.001-.258-.001-.256-.004-.255-.005-.253-.008-.251-.01-.249-.012-.247-.015-.245-.016-.243-.019-.241-.02-.238-.023-.236-.024-.234-.027-.231-.028-.228-.031-.226-.032-.223-.034-.22-.036-.217-.038-.214-.04-.211-.041-.208-.043-.204-.045-.201-.046-.198-.048-.195-.05-.19-.051-.187-.053-.184-.054-.179-.056-.176-.057-.172-.059-.167-.06-.164-.061-.159-.063-.155-.064-.151-.066-.074-.033-.072-.033-.072-.034-.07-.034-.069-.035-.068-.035-.067-.035-.066-.035-.064-.036-.063-.036-.062-.036-.061-.036-.06-.037-.058-.037-.057-.037-.056-.038-.055-.038-.053-.038-.052-.038-.051-.039-.049-.039-.049-.039-.046-.039-.046-.04-.044-.04-.043-.04-.041-.04-.04-.041-.039-.041-.037-.041-.036-.041-.034-.041-.033-.042-.032-.042-.03-.042-.029-.042-.027-.042-.026-.043-.024-.043-.023-.043-.021-.043-.02-.043-.018-.044-.017-.043-.015-.044-.013-.044-.012-.044-.011-.045-.009-.044-.007-.045-.006-.045-.004-.045-.002-.045-.001-.045v-17l.001-.045.002-.045.004-.045.006-.045.007-.045.009-.044.011-.045.012-.044.013-.044.015-.044.017-.043.018-.044.02-.043.021-.043.023-.043.024-.043.026-.043.027-.042.029-.042.03-.042.032-.042.033-.042.034-.041.036-.041.037-.041.039-.041.04-.041.041-.04.043-.04.044-.04.046-.04.046-.039.049-.039.049-.039.051-.039.052-.038.053-.038.055-.038.056-.038.057-.037.058-.037.06-.037.061-.036.062-.036.063-.036.064-.036.066-.035.067-.035.068-.035.069-.035.07-.034.072-.034.072-.033.074-.033.151-.066.155-.064.159-.063.164-.061.167-.06.172-.059.176-.057.179-.056.184-.054.187-.053.19-.051.195-.05.198-.048.201-.046.204-.045.208-.043.211-.041.214-.04.217-.038.22-.036.223-.034.226-.032.228-.031.231-.028.234-.027.236-.024.238-.023.241-.02.243-.019.245-.016.247-.015.249-.012.251-.01.253-.008.255-.005.256-.004.258-.001.258.001zm-9.258 20.499v.01l.001.021.003.021.004.022.005.021.006.022.007.022.009.023.01.022.011.023.012.023.013.023.015.023.016.024.017.023.018.024.019.024.021.024.022.025.023.024.024.025.052.049.056.05.061.051.066.051.07.051.075.051.079.052.084.052.088.052.092.052.097.052.102.051.105.052.11.052.114.051.119.051.123.051.127.05.131.05.135.05.139.048.144.049.147.047.152.047.155.047.16.045.163.045.167.043.171.043.176.041.178.041.183.039.187.039.19.037.194.035.197.035.202.033.204.031.209.03.212.029.216.027.219.025.222.024.226.021.23.02.233.018.236.016.24.015.243.012.246.01.249.008.253.005.256.004.259.001.26-.001.257-.004.254-.005.25-.008.247-.011.244-.012.241-.014.237-.016.233-.018.231-.021.226-.021.224-.024.22-.026.216-.027.212-.028.21-.031.205-.031.202-.034.198-.034.194-.036.191-.037.187-.039.183-.04.179-.04.175-.042.172-.043.168-.044.163-.045.16-.046.155-.046.152-.047.148-.048.143-.049.139-.049.136-.05.131-.05.126-.05.123-.051.118-.052.114-.051.11-.052.106-.052.101-.052.096-.052.092-.052.088-.053.083-.051.079-.052.074-.052.07-.051.065-.051.06-.051.056-.05.051-.05.023-.024.023-.025.021-.024.02-.024.019-.024.018-.024.017-.024.015-.023.014-.024.013-.023.012-.023.01-.023.01-.022.008-.022.006-.022.006-.022.004-.022.004-.021.001-.021.001-.021v-4.127l-.077.055-.08.053-.083.054-.085.053-.087.052-.09.052-.093.051-.095.05-.097.05-.1.049-.102.049-.105.048-.106.047-.109.047-.111.046-.114.045-.115.045-.118.044-.12.043-.122.042-.124.042-.126.041-.128.04-.13.04-.132.038-.134.038-.135.037-.138.037-.139.035-.142.035-.143.034-.144.033-.147.032-.148.031-.15.03-.151.03-.153.029-.154.027-.156.027-.158.026-.159.025-.161.024-.162.023-.163.022-.165.021-.166.02-.167.019-.169.018-.169.017-.171.016-.173.015-.173.014-.175.013-.175.012-.177.011-.178.01-.179.008-.179.008-.181.006-.182.005-.182.004-.184.003-.184.002h-.37l-.184-.002-.184-.003-.182-.004-.182-.005-.181-.006-.179-.008-.179-.008-.178-.01-.176-.011-.176-.012-.175-.013-.173-.014-.172-.015-.171-.016-.17-.017-.169-.018-.167-.019-.166-.02-.165-.021-.163-.022-.162-.023-.161-.024-.159-.025-.157-.026-.156-.027-.155-.027-.153-.029-.151-.03-.15-.03-.148-.031-.146-.032-.145-.033-.143-.034-.141-.035-.14-.035-.137-.037-.136-.037-.134-.038-.132-.038-.13-.04-.128-.04-.126-.041-.124-.042-.122-.042-.12-.044-.117-.043-.116-.045-.113-.045-.112-.046-.109-.047-.106-.047-.105-.048-.102-.049-.1-.049-.097-.05-.095-.05-.093-.052-.09-.051-.087-.052-.085-.053-.083-.054-.08-.054-.077-.054v4.127zm0-5.654v.011l.001.021.003.021.004.021.005.022.006.022.007.022.009.022.01.022.011.023.012.023.013.023.015.024.016.023.017.024.018.024.019.024.021.024.022.024.023.025.024.024.052.05.056.05.061.05.066.051.07.051.075.052.079.051.084.052.088.052.092.052.097.052.102.052.105.052.11.051.114.051.119.052.123.05.127.051.131.05.135.049.139.049.144.048.147.048.152.047.155.046.16.045.163.045.167.044.171.042.176.042.178.04.183.04.187.038.19.037.194.036.197.034.202.033.204.032.209.03.212.028.216.027.219.025.222.024.226.022.23.02.233.018.236.016.24.014.243.012.246.01.249.008.253.006.256.003.259.001.26-.001.257-.003.254-.006.25-.008.247-.01.244-.012.241-.015.237-.016.233-.018.231-.02.226-.022.224-.024.22-.025.216-.027.212-.029.21-.03.205-.032.202-.033.198-.035.194-.036.191-.037.187-.039.183-.039.179-.041.175-.042.172-.043.168-.044.163-.045.16-.045.155-.047.152-.047.148-.048.143-.048.139-.05.136-.049.131-.05.126-.051.123-.051.118-.051.114-.052.11-.052.106-.052.101-.052.096-.052.092-.052.088-.052.083-.052.079-.052.074-.051.07-.052.065-.051.06-.05.056-.051.051-.049.023-.025.023-.024.021-.025.02-.024.019-.024.018-.024.017-.024.015-.023.014-.023.013-.024.012-.022.01-.023.01-.023.008-.022.006-.022.006-.022.004-.021.004-.022.001-.021.001-.021v-4.139l-.077.054-.08.054-.083.054-.085.052-.087.053-.09.051-.093.051-.095.051-.097.05-.1.049-.102.049-.105.048-.106.047-.109.047-.111.046-.114.045-.115.044-.118.044-.12.044-.122.042-.124.042-.126.041-.128.04-.13.039-.132.039-.134.038-.135.037-.138.036-.139.036-.142.035-.143.033-.144.033-.147.033-.148.031-.15.03-.151.03-.153.028-.154.028-.156.027-.158.026-.159.025-.161.024-.162.023-.163.022-.165.021-.166.02-.167.019-.169.018-.169.017-.171.016-.173.015-.173.014-.175.013-.175.012-.177.011-.178.009-.179.009-.179.007-.181.007-.182.005-.182.004-.184.003-.184.002h-.37l-.184-.002-.184-.003-.182-.004-.182-.005-.181-.007-.179-.007-.179-.009-.178-.009-.176-.011-.176-.012-.175-.013-.173-.014-.172-.015-.171-.016-.17-.017-.169-.018-.167-.019-.166-.02-.165-.021-.163-.022-.162-.023-.161-.024-.159-.025-.157-.026-.156-.027-.155-.028-.153-.028-.151-.03-.15-.03-.148-.031-.146-.033-.145-.033-.143-.033-.141-.035-.14-.036-.137-.036-.136-.037-.134-.038-.132-.039-.13-.039-.128-.04-.126-.041-.124-.042-.122-.043-.12-.043-.117-.044-.116-.044-.113-.046-.112-.046-.109-.046-.106-.047-.105-.048-.102-.049-.1-.049-.097-.05-.095-.051-.093-.051-.09-.051-.087-.053-.085-.052-.083-.054-.08-.054-.077-.054v4.139zm0-5.666v.011l.001.02.003.022.004.021.005.022.006.021.007.022.009.023.01.022.011.023.012.023.013.023.015.023.016.024.017.024.018.023.019.024.021.025.022.024.023.024.024.025.052.05.056.05.061.05.066.051.07.051.075.052.079.051.084.052.088.052.092.052.097.052.102.052.105.051.11.052.114.051.119.051.123.051.127.05.131.05.135.05.139.049.144.048.147.048.152.047.155.046.16.045.163.045.167.043.171.043.176.042.178.04.183.04.187.038.19.037.194.036.197.034.202.033.204.032.209.03.212.028.216.027.219.025.222.024.226.021.23.02.233.018.236.017.24.014.243.012.246.01.249.008.253.006.256.003.259.001.26-.001.257-.003.254-.006.25-.008.247-.01.244-.013.241-.014.237-.016.233-.018.231-.02.226-.022.224-.024.22-.025.216-.027.212-.029.21-.03.205-.032.202-.033.198-.035.194-.036.191-.037.187-.039.183-.039.179-.041.175-.042.172-.043.168-.044.163-.045.16-.045.155-.047.152-.047.148-.048.143-.049.139-.049.136-.049.131-.051.126-.05.123-.051.118-.052.114-.051.11-.052.106-.052.101-.052.096-.052.092-.052.088-.052.083-.052.079-.052.074-.052.07-.051.065-.051.06-.051.056-.05.051-.049.023-.025.023-.025.021-.024.02-.024.019-.024.018-.024.017-.024.015-.023.014-.024.013-.023.012-.023.01-.022.01-.023.008-.022.006-.022.006-.022.004-.022.004-.021.001-.021.001-.021v-4.153l-.077.054-.08.054-.083.053-.085.053-.087.053-.09.051-.093.051-.095.051-.097.05-.1.049-.102.048-.105.048-.106.048-.109.046-.111.046-.114.046-.115.044-.118.044-.12.043-.122.043-.124.042-.126.041-.128.04-.13.039-.132.039-.134.038-.135.037-.138.036-.139.036-.142.034-.143.034-.144.033-.147.032-.148.032-.15.03-.151.03-.153.028-.154.028-.156.027-.158.026-.159.024-.161.024-.162.023-.163.023-.165.021-.166.02-.167.019-.169.018-.169.017-.171.016-.173.015-.173.014-.175.013-.175.012-.177.01-.178.01-.179.009-.179.007-.181.006-.182.006-.182.004-.184.003-.184.001-.185.001-.185-.001-.184-.001-.184-.003-.182-.004-.182-.006-.181-.006-.179-.007-.179-.009-.178-.01-.176-.01-.176-.012-.175-.013-.173-.014-.172-.015-.171-.016-.17-.017-.169-.018-.167-.019-.166-.02-.165-.021-.163-.023-.162-.023-.161-.024-.159-.024-.157-.026-.156-.027-.155-.028-.153-.028-.151-.03-.15-.03-.148-.032-.146-.032-.145-.033-.143-.034-.141-.034-.14-.036-.137-.036-.136-.037-.134-.038-.132-.039-.13-.039-.128-.041-.126-.041-.124-.041-.122-.043-.12-.043-.117-.044-.116-.044-.113-.046-.112-.046-.109-.046-.106-.048-.105-.048-.102-.048-.1-.05-.097-.049-.095-.051-.093-.051-.09-.052-.087-.052-.085-.053-.083-.053-.08-.054-.077-.054v4.153zm8.74-8.179l-.257.004-.254.005-.25.008-.247.011-.244.012-.241.014-.237.016-.233.018-.231.021-.226.022-.224.023-.22.026-.216.027-.212.028-.21.031-.205.032-.202.033-.198.034-.194.036-.191.038-.187.038-.183.04-.179.041-.175.042-.172.043-.168.043-.163.045-.16.046-.155.046-.152.048-.148.048-.143.048-.139.049-.136.05-.131.05-.126.051-.123.051-.118.051-.114.052-.11.052-.106.052-.101.052-.096.052-.092.052-.088.052-.083.052-.079.052-.074.051-.07.052-.065.051-.06.05-.056.05-.051.05-.023.025-.023.024-.021.024-.02.025-.019.024-.018.024-.017.023-.015.024-.014.023-.013.023-.012.023-.01.023-.01.022-.008.022-.006.023-.006.021-.004.022-.004.021-.001.021-.001.021.001.021.001.021.004.021.004.022.006.021.006.023.008.022.01.022.01.023.012.023.013.023.014.023.015.024.017.023.018.024.019.024.02.025.021.024.023.024.023.025.051.05.056.05.06.05.065.051.07.052.074.051.079.052.083.052.088.052.092.052.096.052.101.052.106.052.11.052.114.052.118.051.123.051.126.051.131.05.136.05.139.049.143.048.148.048.152.048.155.046.16.046.163.045.168.043.172.043.175.042.179.041.183.04.187.038.191.038.194.036.198.034.202.033.205.032.21.031.212.028.216.027.22.026.224.023.226.022.231.021.233.018.237.016.241.014.244.012.247.011.25.008.254.005.257.004.26.001.26-.001.257-.004.254-.005.25-.008.247-.011.244-.012.241-.014.237-.016.233-.018.231-.021.226-.022.224-.023.22-.026.216-.027.212-.028.21-.031.205-.032.202-.033.198-.034.194-.036.191-.038.187-.038.183-.04.179-.041.175-.042.172-.043.168-.043.163-.045.16-.046.155-.046.152-.048.148-.048.143-.048.139-.049.136-.05.131-.05.126-.051.123-.051.118-.051.114-.052.11-.052.106-.052.101-.052.096-.052.092-.052.088-.052.083-.052.079-.052.074-.051.07-.052.065-.051.06-.05.056-.05.051-.05.023-.025.023-.024.021-.024.02-.025.019-.024.018-.024.017-.023.015-.024.014-.023.013-.023.012-.023.01-.023.01-.022.008-.022.006-.023.006-.021.004-.022.004-.021.001-.021.001-.021-.001-.021-.001-.021-.004-.021-.004-.022-.006-.021-.006-.023-.008-.022-.01-.022-.01-.023-.012-.023-.013-.023-.014-.023-.015-.024-.017-.023-.018-.024-.019-.024-.02-.025-.021-.024-.023-.024-.023-.025-.051-.05-.056-.05-.06-.05-.065-.051-.07-.052-.074-.051-.079-.052-.083-.052-.088-.052-.092-.052-.096-.052-.101-.052-.106-.052-.11-.052-.114-.052-.118-.051-.123-.051-.126-.051-.131-.05-.136-.05-.139-.049-.143-.048-.148-.048-.152-.048-.155-.046-.16-.046-.163-.045-.168-.043-.172-.043-.175-.042-.179-.041-.183-.04-.187-.038-.191-.038-.194-.036-.198-.034-.202-.033-.205-.032-.21-.031-.212-.028-.216-.027-.22-.026-.224-.023-.226-.022-.231-.021-.233-.018-.237-.016-.241-.014-.244-.012-.247-.011-.25-.008-.254-.005-.257-.004-.26-.001-.26.001z"></path>
</symbol>
</defs>
<defs>
<symbol id="clock" width="24" height="24">
<path transform="scale(.5)" d="M12 2c5.514 0 10 4.486 10 10s-4.486 10-10 10-10-4.486-10-10 4.486-10 10-10zm0-2c-6.627 0-12 5.373-12 12s5.373 12 12 12 12-5.373 12-12-5.373-12-12-12zm5.848 12.459c.202.038.202.333.001.372-1.907.361-6.045 1.111-6.547 1.111-.719 0-1.301-.582-1.301-1.301 0-.512.77-5.447 1.125-7.445.034-.192.312-.181.343.014l.985 6.238 5.394 1.011z"></path>
</symbol>
</defs>
<g>
<line id="actor3" x1="75" y1="5" x2="75" y2="528" class="200" stroke-width="0.5px" stroke="#999"></line>
<g id="root-3">
<rect x="0" y="0" fill="#eaeaea" stroke="#666" width="150" height="65" rx="3" ry="3" class="actor"></rect>
<text x="75" y="32.5" dominant-baseline="central" alignment-baseline="central" class="actor" style="text-anchor: middle; font-size: 14px; font-weight: 400; font-family: Open-Sans, sans-serif;">
<tspan x="75" dy="0">
Alice
</tspan>
</text>
</g>
</g>
<g>
<line id="actor4" x1="337" y1="5" x2="337" y2="528" class="200" stroke-width="0.5px" stroke="#999"></line>
<g id="root-4">
<rect x="262" y="0" fill="#eaeaea" stroke="#666" width="150" height="65" rx="3" ry="3" class="actor"></rect>
<text x="337" y="32.5" dominant-baseline="central" alignment-baseline="central" class="actor" style="text-anchor: middle; font-size: 14px; font-weight: 400; font-family: Open-Sans, sans-serif;">
<tspan x="337" dy="0">
John
</tspan>
</text>
</g>
</g>
<g>
<line id="actor5" x1="537" y1="5" x2="537" y2="528" class="200" stroke-width="0.5px" stroke="#999"></line>
<g id="root-5">
<rect x="462" y="0" fill="#eaeaea" stroke="#666" width="150" height="65" rx="3" ry="3" class="actor"></rect>
<text x="537" y="32.5" dominant-baseline="central" alignment-baseline="central" class="actor" style="text-anchor: middle; font-size: 14px; font-weight: 400; font-family: Open-Sans, sans-serif;">
<tspan x="537" dy="0">
Bob
</tspan>
</text>
</g>
</g>
<defs>
<marker id="arrowhead" refx="9" refy="5" markerunits="userSpaceOnUse" markerwidth="12" markerheight="12" orient="auto">
<path d="M 0 0 L 10 5 L 0 10 z"></path>
</marker>
</defs>
<defs>
<marker id="crosshead" markerwidth="15" markerheight="8" orient="auto" refx="16" refy="4">
<path fill="black" stroke="#000000" stroke-width="1px" d="M 9,2 V 6 L16,4 Z" style="stroke-dasharray: 0, 0;"></path>
<path fill="none" stroke="#000000" stroke-width="1px" d="M 0,1 L 6,7 M 6,1 L 0,7" style="stroke-dasharray: 0, 0;"></path>
</marker>
</defs>
<defs>
<marker id="filled-head" refx="18" refy="7" markerwidth="20" markerheight="28" orient="auto">
<path d="M 18,7 L9,13 L14,7 L9,1 Z"></path>
</marker>
</defs>
<defs>
<marker id="sequencenumber" refx="15" refy="15" markerwidth="60" markerheight="40" orient="auto">
<circle cx="15" cy="15" r="6"></circle>
</marker>
</defs>
<text x="206" y="80" text-anchor="middle" dominant-baseline="middle" alignment-baseline="middle" class="messageText" dy="1em" style="font-family: &#34;trebuchet ms&#34;, verdana, arial, sans-serif; font-size: 16px; font-weight: 400;">
Hello John, how are you?
</text>
<line x1="75" y1="117" x2="337" y2="117" class="messageLine0" stroke-width="2" stroke="none" marker-end="url(#arrowhead)" style="fill: none;"></line>
<text x="337" y="178" text-anchor="middle" dominant-baseline="middle" alignment-baseline="middle" class="messageText" dy="1em" style="font-family: &#34;trebuchet ms&#34;, verdana, arial, sans-serif; font-size: 16px; font-weight: 400;">
Fight against hypochondria
</text>
<path d="M 337,215 C 397,205 397,245 337,235" class="messageLine0" stroke-width="2" stroke="none" marker-end="url(#arrowhead)" style="fill: none;"></path>
<g>
<line x1="222" y1="127" x2="452" y2="127" class="loopLine"></line>
<line x1="452" y1="127" x2="452" y2="285" class="loopLine"></line>
<line x1="222" y1="285" x2="452" y2="285" class="loopLine"></line>
<line x1="222" y1="127" x2="222" y2="285" class="loopLine"></line>
<polygon points="222,127 272,127 272,140 263.6,147 222,147" class="labelBox"></polygon>
<text x="247" y="140" text-anchor="middle" dominant-baseline="middle" alignment-baseline="middle" class="labelText" style="font-family: &#34;trebuchet ms&#34;, verdana, arial, sans-serif; font-size: 16px; font-weight: 400;">
loop
</text>
<text x="362" y="145" text-anchor="middle" class="loopText" style="font-family: &#34;trebuchet ms&#34;, verdana, arial, sans-serif; font-size: 16px; font-weight: 400;">
<tspan x="362">
[Healthcheck]
</tspan>
</text>
</g>
<g>
<rect x="362" y="295" fill="#EDF2AE" stroke="#666" width="150" height="37" rx="0" ry="0" class="note"></rect>
<text x="437" y="300" text-anchor="middle" dominant-baseline="middle" alignment-baseline="middle" class="noteText" dy="1em" style="font-family: &#34;trebuchet ms&#34;, verdana, arial, sans-serif; font-size: 14px; font-weight: 400;">
<tspan x="437">
Rational thoughts!
</tspan>
</text>
</g>
<text x="206" y="347" text-anchor="middle" dominant-baseline="middle" alignment-baseline="middle" class="messageText" dy="1em" style="font-family: &#34;trebuchet ms&#34;, verdana, arial, sans-serif; font-size: 16px; font-weight: 400;">
Great!
</text>
<line x1="337" y1="384" x2="75" y2="384" class="messageLine1" stroke-width="2" stroke="none" marker-end="url(#arrowhead)" style="stroke-dasharray: 3, 3; fill: none;"></line>
<text x="437" y="399" text-anchor="middle" dominant-baseline="middle" alignment-baseline="middle" class="messageText" dy="1em" style="font-family: &#34;trebuchet ms&#34;, verdana, arial, sans-serif; font-size: 16px; font-weight: 400;">
How about you?
</text>
<line x1="337" y1="436" x2="537" y2="436" class="messageLine0" stroke-width="2" stroke="none" marker-end="url(#arrowhead)" style="fill: none;"></line>
<text x="437" y="451" text-anchor="middle" dominant-baseline="middle" alignment-baseline="middle" class="messageText" dy="1em" style="font-family: &#34;trebuchet ms&#34;, verdana, arial, sans-serif; font-size: 16px; font-weight: 400;">
Jolly good!
</text>
<line x1="537" y1="488" x2="337" y2="488" class="messageLine1" stroke-width="2" stroke="none" marker-end="url(#arrowhead)" style="stroke-dasharray: 3, 3; fill: none;"></line>
<g>
<rect x="0" y="508" fill="#eaeaea" stroke="#666" width="150" height="65" rx="3" ry="3" class="actor"></rect>
<text x="75" y="540.5" dominant-baseline="central" alignment-baseline="central" class="actor" style="text-anchor: middle; font-size: 14px; font-weight: 400; font-family: Open-Sans, sans-serif;">
<tspan x="75" dy="0">
Alice
</tspan>
</text>
</g>
<g>
<rect x="262" y="508" fill="#eaeaea" stroke="#666" width="150" height="65" rx="3" ry="3" class="actor"></rect>
<text x="337" y="540.5" dominant-baseline="central" alignment-baseline="central" class="actor" style="text-anchor: middle; font-size: 14px; font-weight: 400; font-family: Open-Sans, sans-serif;">
<tspan x="337" dy="0">
John
</tspan>
</text>
</g>
<g>
<rect x="462" y="508" fill="#eaeaea" stroke="#666" width="150" height="65" rx="3" ry="3" class="actor"></rect>
<text x="537" y="540.5" dominant-baseline="central" alignment-baseline="central" class="actor" style="text-anchor: middle; font-size: 14px; font-weight: 400; font-family: Open-Sans, sans-serif;">
<tspan x="537" dy="0">
Bob
</tspan>
</text>
</g>
</svg>
</div>
</blockquote>
<h2><a id="_269"></a>数学公式</h2>
<p>支持 LaTeX 编辑显示支持&#xff0c;<br /> 使用 <code>$</code> 表示&#xff0c;其中一个 <code>$</code> 表示在行内&#xff0c;两个 <code>$</code> 表示独占一行。</p>
<blockquote>
<p>eg : <span class="katex--inline"><span class="katex"><span class="katex-mathml">





∑



i


&#61;


1



n




a


i



&#61;


0



\sum_{i&#61;1}^n a_i&#61;0


</span><span class="katex-html"><span class="base"><span class="strut" style="height: 1.104em; vertical-align: -0.29971em;"></span><span class="mop"><span class="mop op-symbol small-op" style="position: relative; top: -5e-06em;">∑</span><span class="msupsub"><span class="vlist-t vlist-t2"><span class="vlist-r"><span class="vlist" style="height: 0.804292em;"><span class="" style="top: -2.40029em; margin-left: 0em; margin-right: 0.05em;"><span class="pstrut" style="height: 2.7em;"></span><span class="sizing reset-size6 size3 mtight"><span class="mord mtight"><span class="mord mathdefault mtight">i</span><span class="mrel mtight">&#61;</span><span class="mord mtight">1</span></span></span></span><span class="" style="top: -3.2029em; margin-right: 0.05em;"><span class="pstrut" style="height: 2.7em;"></span><span class="sizing reset-size6 size3 mtight"><span class="mord mathdefault mtight">n</span></span></span></span><span class="vlist-s">​</span></span><span class="vlist-r"><span class="vlist" style="height: 0.29971em;"><span class=""></span></span></span></span></span></span><span class="mspace" style="margin-right: 0.166667em;"></span><span class="mord"><span class="mord mathdefault">a</span><span class="msupsub"><span class="vlist-t vlist-t2"><span class="vlist-r"><span class="vlist" style="height: 0.311664em;"><span class="" style="top: -2.55em; margin-left: 0em; margin-right: 0.05em;"><span class="pstrut" style="height: 2.7em;"></span><span class="sizing reset-size6 size3 mtight"><span class="mord mathdefault mtight">i</span></span></span></span><span class="vlist-s">​</span></span><span class="vlist-r"><span class="vlist" style="height: 0.15em;"><span class=""></span></span></span></span></span></span><span class="mspace" style="margin-right: 0.277778em;"></span><span class="mrel">&#61;</span><span class="mspace" style="margin-right: 0.277778em;"></span></span><span class="base"><span class="strut" style="height: 0.64444em; vertical-align: 0em;"></span><span class="mord">0</span></span></span></span></span></p>
</blockquote>
<p>参考教程&#xff1a;https://1024th.github.io/MathJax_Tutorial_CN</p>
<p>推荐一个常用的数学公式在线编译网站&#xff1a;https://www.latexlive.com</p>
<h2><a id="HTML_281"></a>HTML引用</h2>
<p>直接在Markdown里面写HTML即可</p>
<h3><a id="CSS__283"></a>CSS 样式相关</h3>
<h4><a id="_284"></a>样式标签</h4>
<blockquote>
<p>&lt;b&gt;加粗&lt;/b&gt;<br /> &lt;strong&gt;加粗&lt;/strong&gt;<br /> &lt;i&gt;倾斜&lt;/i&gt;<br /> &lt;em&gt;倾斜&lt;/em&gt;<br /> &lt;u&gt;下划线&lt;/u&gt;<br /> &lt;ins&gt;下划线&lt;/ins&gt;<br /> &lt;s&gt;删除线&lt;/s&gt;<br /> &lt;del&gt;删除线&lt;/del&gt;<br /> &lt;sub&gt;下标&lt;/sub&gt;<br /> &lt;sup&gt;上标&lt;/sup&gt;</p>
</blockquote>
<h4><a id="_297"></a>内联样式</h4>
<blockquote>
<p>&lt;b style&#61;“font-size:80px; color:red”&gt;加粗&lt;/b&gt;</p>
</blockquote>
<h4><a id="style_299"></a>&lt;style&gt;标签</h4>
<blockquote>
<p>&lt;style&gt;<br /> h1{<!-- --><br /> font-size:80px;<br /> color:#7ecef4;<br /> text-intent:10px;<br /> }<br /> &lt;/style&gt;</p>
</blockquote>
<h4><a id="linkCSS_307"></a>&lt;link&gt;引用外部CSS</h4>
<blockquote>
<p>&lt;link href&#61;“main.css” rel&#61;“stylesheet”&gt;</p>
</blockquote>
<p>这种方式&#xff0c;某些Markdown渲染器可以&#xff0c;反正obsidian是不行</p>
<h3><a id="HTML__312"></a>HTML 内容相关</h3>
<p>在Markdown中可以展示出网页内容<br /> 支持的也就是普通的内容&#xff0c;交互式的标签基本都被和谐了<br /> HTML教程&#xff1a;https://www.runoob.com/html/html-tutorial.html</p>
<blockquote>
<p><strong>例子&#xff0c;用html的 <code>&lt;a&gt;</code> 和 <code>&lt;img&gt;</code> 标签实现带连接的图片</strong></p>
</blockquote>
<blockquote>
<p>&lt;a href &#61;“超链接地址”&gt;&lt;img src&#61;“图片地址”&gt;&lt;/a&gt;</p>
</blockquote>
<h3><a id="JavaScript__320"></a>JavaScript 脚本相关</h3>
<p>很多Markdown渲染器是不允许js跑起来的</p>
<blockquote>
<p><strong>外部引用和直接写这两种基本都跑不起来</strong><br /> &lt;script src&#61;“javascript.js”&gt;&lt;/script&gt;</p>
<p>&lt;script&gt;<br /> console.log(“hello world!”)<br /> &lt;/script&gt;</p>
</blockquote>
<blockquote>
<p><strong>内联事件的js可能可以跑起来,反正obsidian是不行</strong><br /> &lt;div οnclick&#61;“(function(){ alert(1)})()”&gt;js测试按钮&lt;/div&gt;</p>
</blockquote>
<h2><a id="_334"></a>反斜杠转义</h2>
<p>由于Markdown的语法基本都是用的符号表示&#xff0c;所以当需要直接输出某些特定的符号的时候&#xff0c;就必须使用反斜杠的转义作用了&#xff0c;使用方法很简单&#xff0c;跟大部分的编程语言的用法一样&#xff0c;只需要在特定的符号前面加上一个反斜杠就可以了&#xff0c;例如输出<code>\</code>本身&#xff0c;就需要使用<code>\\</code>来表示了。</p>
<h2><a id="Todo_List_338"></a>Todo List</h2>
<p><code>-/&#43;/*</code>&#43;<code>空格</code>&#43;<code>[</code>&#43;<code>空格/x</code>&#43;<code>]</code> &#43;<code>空格</code>&#43;文字内容</p>
<blockquote>
<p><strong>语法</strong></p>
</blockquote>
<blockquote>
<p>- [ ] 待办事项<br /> - [x] 已完成的待办事项</p>
</blockquote>
<blockquote>
<p><strong>实例</strong></p>
</blockquote>
<blockquote>
<ul><li class="task-list-item"><input type="checkbox" class="task-list-item-checkbox" disabled="disabled" /> 待办事项</li><li class="task-list-item"><input type="checkbox" class="task-list-item-checkbox" checked="true" disabled="disabled" /> 已完成的待办事项</li></ul>
</blockquote>
<h2><a id="_351"></a>脚注</h2>
<p>在文档末尾写上<code>[</code>&#43;<code>^&#43;数字</code>&#43;<code>]:</code>&#43;文字内容 声明一个脚注<br /> 然后就跟文献引用一样&#xff0c;在要引用该脚注的文字后插入<code>[</code>&#43;<code>^&#43;数字</code>&#43;<code>]</code>即可</p>
<blockquote>
<p><strong>语法</strong></p>
</blockquote>
<blockquote>
<p>该方法根据实验证明有效[^1]<br /> [^1]:文章链接</p>
</blockquote>
<hr />
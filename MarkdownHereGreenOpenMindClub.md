/*说明:


~ 开智部落御用 CSS 小清新格式 2016-10-14 更新
~ 使用说明文档见 https://github.com/OpenMindClub/OpenMind.Social/wiki/HBOpenMindStyle

### 正文设置

- 在「P」字段设置
- 正文字号：14
- 行距(line-height)：1.75倍
- 左右段落距（padding-right/left）：0.7 毫米
- 上下段落距(padding-top/bottom)：0.5 毫米
- 颜色color：#3e3e3e


### 引用字体

- 颜色color：rgb(136, 136, 136)

### 标题设置

- 在「h」字段设置
- 大标题(h1)：20 字号、加粗、置中、蓝色：基本不用
- 二级标题(h2)：18 字号、加粗、置中：常用，分组块用
- 三级标题(h3) 17 字号、加粗：偶尔用，做小标题
- 四级标题(h4) 15 字号、加粗，有颜色：画重点用
- 五级标题(h5) 14 字号、灰色：用于摘要和介绍
- 六级标题(h6) 15 字号、底线黑色横条：用于标注相关文章，可容纳 6 个以内文字

### 无/有序行距

- 无/有序行距(li/margin)：0.5毫米
- 颜色color：#3e3e3e


### 注意事项：

- 请在纯文本状态下编辑文字，在已转化的文本下再编辑会造成格式错乱。
	+ 这不是 Markdown Here 的 Bug 而是 Markdown Here 本身的设定
	+ 为何如此设定？我也不知道。

### 自定义 CSS 设置不起作用

试试在后面补上!important，就好像这样：

h2 {
  font-size: 20px !important;
}


### 参考链接：

- [Markdown Here](http://markdown-here.com/get.html)
- [你知道吗，在印象笔记里也能用 Markdown 写作 - Matrix](http://matrix.sspai.com/p/b768d1e0)

### Changlog

- 2018-02-02 HYL： 这是CSS，可以用来渲染
- 2016-09-30 陈素封修订一级标题颜色
- 2016-09-27 曹帅修订
- 2016-09-09 修订为小清新版
- 2016-07-25 调整正文字体为16号，修正部分错误
- 2016-06-23 调整正文字体为16号，正文行距为1.75
- 2016-05-08 陈素封创建

*/ 

pre {
	font-size: 1em;
	line-height: 1.2em;
	font-size: 14px;
	color: #3e3e3e;
	padding-top: 0.5em;
	padding-bottom: 0.5em;
	padding-right: 2em;
	padding-left: 2em;
}

pre code {
	white-space: pre;
	overflow: auto;
}

table, pre, dl, blockquote, q, ul, ol {
	margin: 1.2em 0;
}

ul, ol {
	padding-left: 3em;
	font-size: 14px!important;
    padding-right: 2em;
}

li {
	margin: 0.3em 0;
	line-height: 2em;
	font-size: 14px!important;
	color: #3e3e3e;
 /*无序和有序的行距*/
}

ul ul, ul ol, ol ul, ol ol {
	margin: 0;
	padding-left: 1.2em;
}

ul ul, ul, ul {
	list-style-type: square;
	font-size: 14px;
}

ol ol, ul ol {
	list-style-type: lower-roman;
}

ul ul ol, ul ol ol, ol ul ol, ol ol ol {
	list-style-type: lower-alpha;
}

dl {
	padding: 0;
	color: #3e3e3e;
}

dl dt {
	font-size: 1em;
	color: #3e3e3e;
	font-style: italic;
}

dl dd {
	margin: 0 0 1em;
	padding: 0 1em;
	color: #3e3e3e;
}

blockquote > p {
        padding-left: 1em!important;
        padding-right: 1em!important;
}

blockquote, q {
	border-left: 4px solid #888;
	padding: 0 0.5em;
	line-height: 2.2em;
	color: #888!important;
	quotes: none!important;
	padding-right: 0.5em;
	padding-left: 0.5em;
	margin: 1em;
	 /*引用*/
}

blockquote::before, blockquote::after, q::before, q::after {
	content: none;
}

h1, h2, h3, h4, h5, h6 {
	margin: 1.3em 0 1em;
	padding: 0;
	font-weight: bold;
}

h1 {
	font-size: 20px;
	color: #49b34f;
	padding-right: 1.2em;
	padding-left: 1.2em;
	text-align: center;
}

h2 {
	font-size: 18px;
	color: #49b34f;
	padding-right: 1.2em;
	padding-left: 1.2em;
	text-align: center;
}

h3 {
	font-size: 16px;
	padding-right: 1.2em;
	padding-left: 1.2em;
}

h4 {
	font-size: 14px;
	color: #49b34f;
	padding-right: 1.2em;
	padding-left: 1.2em;
	text-align: center;
}

h5 {
	font-size: 14px;
	padding-top: 15px;
	padding-right: 15px;
	padding-bottom: 15px;
	padding-left: 15px;
	box-shadow: rgb(170, 170, 170) 0px 0px 3px;
	color: #777;
	font-weight: 400;
	line-height: 1.75em;
}

h6 {
	font-size: 15px;
	padding-right: 1.2em;
	padding-left: 1.2em;
	border-bottom: 2px solid rgb(42, 52, 58);
	width: 120px
}

table {
	padding: 0;
	border-collapse: collapse;
	border-spacing: 0;
	font-size: 1em;
	font: inherit;
	border: 0;
}

tbody {
	margin: 0;
	padding: 0;
	border: 0;
}

table tr {
	border: 0;
	border-top: 1px solid #CCC;
	background-color: white;
	margin: 0;
	padding: 0;
}

table tr:nth-child(2n) {
	background-color: #F8F8F8;
}

table tr th, table tr td {
	font-size: 1em;
	border: 1px solid #CCC;
	margin: 0;
	padding: 0.5em 1em;
}

table tr th {
	font-weight: bold;
	background-color: #F0F0F0;
}

p {
	font-size: 14px;
	line-height: 2em;
	padding-top: 0.5em;
	padding-bottom: 0.5em;
	padding-right: 1.2em;
	padding-left: 1.2em;
}；

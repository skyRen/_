## 概
>	- 区块元素  
>		>	1\. 段落和换行  
>			2\. 标题  
>			3\. 区块引用 `Blockquote`  
>			4\. 列表  
>			5\. 代码区块  
>			6\. 分割线
>
>	- 区段元素  
>		>	1\. 链接  
>			2\. 强调  
>			3\. 代码  
>			4\. 图片
>
>	- 其他  
>		>	1\. 自动链接  
>			2\. 反斜杠  
>			3\. 表格


## 区块元素
1. ### 段落和换行
	- Markdown 段落是有连续的文本行组成，前后要有至少一个**空行**。
	- 强制换行是末尾加上2个或以上空格，再换行。

2. ### 标题
	- 两种标题语法：类`Setext`和类`axt`形式。  
		+ 类`Setext`形式，任意多个“=”（高阶标题）和“-”（低阶标题）为底线。
		+ 类`axt`形式，1\~6个“#”为开头，代表 h1\~h6。

3. ### 区块引用 Blockquote
	- 用“>”在段落开头行或每一行，可形成区块。
	- 区块可以嵌套区块。
	- 区块内可以使用其他 Markdown 语法，例如：标题，列表等。

4. ### 列表
	- 无序列表，行开头使用 星号（*）、加号（+）、减号（-）。
	- 有序列表，行开头使用 “数字+英文dot”。

5. ### 代码区块
	- 行开头 4个空格 缩进，即为代码区块。

6. ### 分割线
	- 三个以上的 星号（*）、减号（-）、下划线（_）单独占一行，即可形成分割线。
	- 其中，* 和 -，中间可以有空格。

## 区段元素
1. ### 链接
	- 支持，行内式 和 参考式，title 可选。
	- 行内式，`[label](url "title")`。
	- 参考式，`[label][id]`，然后在段落之后，另起一段，写入参考详情，`[id]: url "title"`。  
		注：id 可以为空，即， `[label][]`  参考详情， `[label]: url "title"`。  

	例：
	```
	I get 10 times more traffic from [Google][1] than from [Yahoo][2] or [MSN][3].

	  [1]: http://google.com/        "Google"
	  [2]: http://search.yahoo.com/  "Yahoo Search"
	  [3]: http://search.msn.com/    "MSN Search"
	```
	等同于：
	```
	I get 10 times more traffic from [Google][] than from [Yahoo][] or [MSN][].

	  [Google]: http://google.com/       "Google"
	  [Yahoo]: http://search.yahoo.com/  "Yahoo Search"
	  [MSN]: http://search.msn.com/      "MSN Search"
	```

2. ### 强调
	- 文本前后存在 下划线（_）和 星号（*），则文本内容为强调。
	- 文本前后一个强调符号为*斜体*，两个为**粗体**。

3. ### 代码
	- 被 “\`” 包括，可显示为代码格式，可多个 “\`”。

4. ### 图片
	- 也支持两种方式，行内式 和 参考式。
	- 行内式，`![Alt text](/path/to/img.jpg "Optional title")`。
	- 参考式，`![Alt text][id]`，参考详情，`[id]: url/to/image  "Optional title attribute"`。

## 其他
1. ### 自动链接
	- Markdown 支持简短的方式，转换 url 和 email。
	- `<http://example.com>` 或 `address@example.com`;

2. ### 反斜杠
	- Markdown 用 反斜杠（\）转换特殊意义的字符。
	- 如下：  
	```
	\   反斜线
	`   反引号
	*   星号
	_   底线
	{}  花括号
	[]  方括号
	()  括弧
	#   井字号
	+   加号
	-   减号
	.   英文句点
	!   惊叹号
	```
3. ### 表格
	- 例：
	```
	| Tables        | Are           | Cool  |
	| ------------- |:-------------:| -----:|
	| col 3 is      | right-aligned | $1600 |
	| col 2 is      | centered      |   $12 |
	| zebra stripes | are neat      |    $1 |
	```
	展示：

	| Tables        | Are           | Cool  |
	| ------------- |:-------------:| -----:|
	| col 3 is      | right-aligned | $1600 |
	| col 2 is      | centered      |   $12 |
	| zebra stripes | are neat      |    $1 |









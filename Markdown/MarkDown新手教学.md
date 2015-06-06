##
###

(空行才换行，普通的换行不换行）

	you are good.
	I like you.
you are good.
I like you.

	you are good.

	I like you.
you are good 

I like you.


##
#A First 标题

	#A First

## A Second 标题
	## A Second


##
###区块###
用>符号引出

	>aaaaaaaaa

	>bbbbbbbbbb
>aaaaaaaaa

>bbbbbbbbbb

--------------------
###强调
*或_ 包起来的 *斜体*

** 或 __包起来的: **粗体**

    You are such *fucking* man.

	You are such _fucking_ man.

	You are such **fucking** man.

	You are such __fucking__ man.
You are such *fucking* man.

You are such _fucking_ man.

You are such **fucking** man.

You are such __fucking__ man.

--------------------
###列表
开头用*, +, -, 都可以

	* 11111
	* 222222
	* 33333
* 11111
* 222222
* 33333

带数字的用**数字加英文.**
(看着好像跟输入似的，实际会自动编号缩进）

	1. 11111
	2. 222222
	3. 33333

1. 11111
2. 222222
3. 33333

缩进用Tab

	* A list item.
	With multiple paragraphs.
		* Another item in the list.
* A list item.
With multiple paragraphs.
	* Another item in the list.

##
###链接
用括号 [ 给出关键字，（ 给出地址

	Go to the [YyisGod](https://github.com/yyisgod)
Go to the [YyisGod](https://github.com/yyisgod)

加上title,在链接用"号框起来

	Go to the [YyisGod](https://github.com/yyisgod "Yy")
Go to the [YyisGod](https://github.com/yyisgod "Yy's Git")

引用类型的链接,在关键字后用[ 定义名称，之后为其定义,名称不分大小写

	I get 10 times more traffic from [Google][1] than from
	[Yahoo][2] or [MSN][3].[Git][g].

	[1]: http://google.com/ "Google"
	[2]: http://search.yahoo.com/ "Yahoo Search"
	[3]: http://search.msn.com/ "MSN Search
	[g]: https://github.com/yyisgod "Yy's Git"
I get 10 times more traffic from [Google][1] than from
[Yahoo][2] or [MSN][3].[Git][g].

[1]: http://google.com/ "Google"
[2]: http://search.yahoo.com/ "Yahoo Search"
[3]: http://search.msn.com/ "MSN Search"
[g]: https://github.com/yyisgod "Yy's Git"

##
###图片
与链接很像，前面多个叹号!,只不过地址是图片的。

	![alt text](/path/to/img.jpg "Title")
	引用形式:
	![alt text][id]
	[id]: /path/to/img.jpg "Title"
![git](http://c.hiphotos.baidu.com/baike/w%3D268/sign=48706442f0d3572c66e29bdab2126352/f7246b600c338744a9591cd7530fd9f9d62aa0f8.jpg "git")

##
###代码
反引号`用来框住代码词

	you are `<int>`
you are `<int>`

一个Tab（4个空格）将该行视为代码

	int i = 0


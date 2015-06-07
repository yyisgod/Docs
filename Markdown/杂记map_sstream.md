***
#杂记 map和sstream
##
	map<int,X> m;
此时如果直接调用

	X x = m[i];
如果 对应的X对象没有创建，则会自动创建一个。

不过如果按照上面这种写法，只是得到了对象的复制而已，如果要操作map中存储的对象，需要这样写：

	X* x = &m[i];

##
**sstream**拿来控制输出不错，比如输出格式
>a,b,c,d,e
循环肯定会这么写

	cout << ch << ',';
这样就会多出来逗号了。
此时不如使用`sstream`来作中转，再输出到`string`方便调整

	sstream ss;
	ss << ch << ',';
	string str;
	ss >> str;
	cout << str.substr(0,str.length()-1);


 
 
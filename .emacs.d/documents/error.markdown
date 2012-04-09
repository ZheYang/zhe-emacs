# C语言中#error和#warning的作用

## #error的使用

* 强制终止编译，常用于程序调试
* 发布源码时，提示开发者修改必要信息。比如：

	    #error : Change this value to your Flickr key
    
     	NSString *const FlickrAPIKey = @"your-key-here";

当开发者拿到源码，没有修改配置就编译，就会报错：

![编译报错](/home/user/.emacs.d/documents/img/error.png "效果")

* 短时间离开电脑时做标记

	  #error : Check this code first

这样，回来时就可以轻松找到上次的位置

## #warning的使用

* \#warning的使用和#error一样，不过#warning会把警告信息输出，但不会打断编译过程

*  *#warning还能这样玩*--用#warning来记录TODO和FixMe

## 参考资料
1. [Using #error and #warning Compiler Directives][1]   John Muchow
2. [预编译和宏定义][2]
3. [#error 等其他常用预处理命令][3]

[1]: <http://iphonedevelopertips.com/c/using-error-and-warning-compiler-directives.html>
[2]: http://www.neu.edu.cn/cxsj/online/C11/ch11_5_1.html
[3]: http://book.51cto.com/art/201107/277759.htm

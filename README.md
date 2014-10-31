IR
==

Information Retrieval Project

- 2014-10-31 重大修改。因为直接使用宏定义很有局限性，因此改成了函数。头文件见kit/IRLog.h，源文件见kit/IRLog.cpp。
使用方法:把头文件和源文件和你的代码放在一起，然后正常编译即可。也可以只用已经编译好的IRLog.a，在代码中引入IRLog.h，编译的时候加入编译选项 -lIRLog -L. 即可，可以在kit目录下测试:
		g++ main.cpp -lIRLog -L. 
		./a.out

- 2014-10-30 统一日志和错误的输出，标准头文件见kit/IRLog.h，写代码如果需要打印日志就可以include这个头文件，需要在可执行文件的目录下建立log和err两个目录，详情见头文件中的注释。

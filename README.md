[目录说明]<br>
.<br>
├── app 			测试程序代码目录<br>
├── doxygen.conf	Doxygen配置文件<br>
├── GenOutPut.sh	编译脚本<br>
├── Inc				头文件目录<br>
├── Lib				库文件目录<br>
├── Makefile<br>
├── Objs			编译中间文件目录<br>
├── Output			输出面向用户的文件<br>
├── Readme			说明文档<br>
└── Src				源码目录<br>
<br>
<br>
[编译接口库]<br>
如果只需要现成的静态库，直接参看Output目录。当用户对代码进行修改后，直接运行脚本GenOutput.sh，编译结果和自动生成的Doxygen文档自动放入Output目录。<br>
<br>
[库文件说明]<br>
libosAdaption.a：OS接口封装库，封装内容参见头文件，位于include/osAdaption目录<br>
libRestFulLinux.a：Restful方式功能封装接口<br>
<br>
[用户程序编译]<br>
用户编译自己的程序时请链接上述两个库和数学库(-losAdaption -lRestfulLinux -lm)，参见app/test.c line14<br>


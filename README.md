# JAVA-虚拟机<br>
##（1）运行时数据区域<br>
java虚拟机在执行代码过程中会把所管理的内存划分为若干个不同的数据区域。<br>
这些区域有各自用途，以及创建和销毁的时间，有的区域随着虚拟机进程的启动而存在，<br>
有的区域依赖用户进程的启动结束而创建和销毁。<br>
运行时数据区域大致划分大致为：<br>
1，程序计数器<br>
2，java虚拟机栈<br>
3，方法区<br>
4，本地方法栈<br>
5，堆<br>
![Image text](https://raw.githubusercontent.com/hongmaju/light7Local/master/img/productShow/20170518152848.png)

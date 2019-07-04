JAVA-虚拟机
------------------------------
### （1）运行时数据区域<br>
java虚拟机在执行代码过程中会把所管理的内存划分为若干个不同的数据区域。<br>
这些区域有各自用途，以及创建和销毁的时间，有的区域随着虚拟机进程的启动而存在，<br>
有的区域依赖用户进程的启动结束而创建和销毁。<br>
运行时数据区域大致划分大致为：程序计数器，java虚拟机栈，方法区，本地方法栈，堆<br>

<br>
![Image text](https://github.com/funaifu/JAVA-/blob/master/imge/java%E8%BF%90%E8%A1%8C%E6%97%B6%E6%95%B0%E6%8D%AE%E5%9C%A8%E5%86%85%E5%AD%98%E4%B8%AD%E7%9A%84%E5%88%86%E9%85%8D.jpg)<br>
<br>
![Image text](https://github.com/funaifu/JAVA-/blob/master/imge/java%E5%A0%86%E5%86%85%E5%AD%98%E8%AF%A6%E7%BB%86%E5%88%86%E9%85%8D.jpg)<br>
<br>
#### 四级标题  <br>
### 1，程序计数器<br>
 程序计数器，线程私有，


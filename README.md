JAVA-虚拟机
------------------------------
### （1）运行时数据区域<br>
java虚拟机在执行代码过程中会把所管理的内存划分为若干个不同的数据区域。<br>
这些区域有各自用途，以及创建和销毁的时间，有的区域随着虚拟机进程的启动而存在，<br>
有的区域依赖用户进程的启动结束而创建和销毁。<br>
运行时数据区域大致划分大致为：程序计数器，java虚拟机栈，方法区，本地方法栈，堆<br>

<br>
![add Image](https://github.com/funaifu/JAVA-/blob/master/imge/java%E8%BF%90%E8%A1%8C%E6%97%B6%E6%95%B0%E6%8D%AE%E5%9C%A8%E5%86%85%E5%AD%98%E4%B8%AD%E7%9A%84%E5%88%86%E9%85%8D.jpg)<br>
<br>
![add Image](https://github.com/funaifu/JAVA-/blob/master/imge/java%E5%A0%86%E5%86%85%E5%AD%98%E8%AF%A6%E7%BB%86%E5%88%86%E9%85%8D.jpg)
<br>

##### 程序计数器<br>
程序计数器是一块较小的内存空间，他可以看做是当前线程所执行的字节码的行号指示器；在虚拟机的概念模型里（仅仅是概念模型，各种虚拟机可能会通过一些<br>更高效的方式实现），字节码解释器工作时，就是通过改变这个计数器值来选取下一条执行字节码指令，分支，循环，跳转，异常处理，线程恢复等基础功能都需要依赖这个计数器来完成。<br>————————摘抄自 周志明版《深入理解java虚拟机》<br>
他的特点有：
* 线程私有
* java虚拟机规范里面，唯一一个没有规定任何OutOfMemoryError情况的区域
* 生命周期随着线程，线程启动而产生，线程结束而消亡
<br>
![add Image](https://github.com/funaifu/JAVA-/blob/master/imge/java%E5%AD%97%E8%8A%82%E7%A0%81%E6%8C%87%E4%BB%A4.jpg)
<br>
如图： Code:下面的   0: iconst_1 其中0就是代表程序计数器记录的字节码执行指令， LineNumberTable: 下面代表的是执行指令对应的源代码行号。<br>


# Jvm初始启动时有几个线程

1、Finalizer 线程的任务就是调用finalize\(\)方法来进行垃圾回收。

2、Signal Dispatcher 线程的任务就是处理[操作系统](http://lib.csdn.net/base/operatingsystem)方面的东西，屏蔽操作系统，使Java达到跨平台的事儿应该是它干的。

3、Reference Handler线程的任务就是将一个不用的对象打上标记，放到回收对象的队列中，以便于Finalizer线程来进行释放内存操作。

4、Main线程


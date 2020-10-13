# Visual simulation of process-scheduling
project in school

--------------------
This system is completed by visual studio 2017 C#. After the program runs, it needs to 
input process information and select scheduling method, and finally outputs the results. 

First of all, we need to input two information of the process: process name, arrival time and demand time. and then select process scheduling, 
job scheduling method, and memory size. After input, the main functions of the system are realized, which can be roughly divided into three main modules:

1. It can move the process into the external memory, judge the timing of process scheduling and job scheduling, and complete the framework of the main program

2. Process scheduling:
 - FIFO, select the process with the earliest arrival time in external memory and put it into memory.
 - SJF, select the process that needs the least time in external memory and put it into memory.
 - Hrrn, select the process with the highest response ratio in external memory and put it into memory.

3. Job scheduling:
 - FIFO, which executes the process with the earliest arrival time in memory.
 - RR, only execute the process of queue head in memory. When the process in memory executes to a given time slice,
 the current process will be blocked and put at the end of the queue, and then the process of queue head will be executed.

The status of each process in each unit of time will be displayed in a graphical interface.

---------------------

# 可视化进程调度

此系统用visual studio 2017 C#完成，程序运行后需要输入进程信息与选择调度方法，最后输出结果。

首先需要输入进程两个信息：进程名，到达时间以及需求时间。然后是选择进程调度，作业调度的方式和内存的大小。输入完后就是系统的主要功能实现，大致分为三个主要模块：

1. 实现将进程移入外存，以及判断进程调度与作业调度的时机，完成主程序的框架

2. 进程调度：
 - FIFO，选出外存中到达时间最早的进程放入内存中。
 - SJF，选出外存中需求时间最少的进程放入内存中。
 - HRRN，选出外存中响应比最高的进程放入内存中。


3. 作业调度：
 - FIFO，执行内存中到达时间最早的进程。
 - RR，只执行内存中队头的进程，当内存中的进程执行到一个给定的时间片后便将当前进程阻断并放到队列末尾然后再执行队头的进程。

每一单位时间中的每个进程的状况都将以图形界面展示出来。

# 简介

         Hadoop Map/Reduce是一个使用简易的软件框架，基于它写出来的应用程序能够运行在由上千个商用机器组成的大型集群上，并以一种可靠容错的方式并行处理上T级别的数据集。

        一个Map/Reduce _作业（job）_ 通常会把输入的数据集切分为若干独立的数据块，由 _map任务（task）_以完全并行的方式处理它们。框架会对map的输出先进行排序， 然后把结果输入给_reduce任务_。通常作业的输入和输出都会被存储在文件系统中。 整个框架负责任务的调度和监控，以及重新执行已经失败的任务。

         通常，Map/Reduce框架和分布式文件系统是运行在一组相同的节点上的，也就是说，计算节点和存储节点通常在一起。这种配置允许框架在那些已经存好数据的节点上高效地调度任务，这可以使整个集群的网络带宽被非常高效地利用。

![MapReduce&#x6846;&#x67B6;&#x8FDB;&#x884C;&#x8BCD;&#x9891;&#x7EDF;&#x8BA1;](../.gitbook/assets/image%20%281%29.png)




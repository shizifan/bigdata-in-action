# 简介

## 介绍

在2003，2004和2006这三年中，Google连续发表了三篇大数据领域重量级的论文：GFS（Google File System），MapReduce和BigTable。基于这三篇论文，Doug Cutting在一个大型全网搜索引擎（[Nutch](http://nutch.apache.org/)）项目中实现了DFS和MapReduce。之后Doug Cutting加入了Yahoo，该项目也被独立出来命名为[Hadoop](https://hadoop.apache.org/)，成为了Apache的顶级开源项目，大数据技术由此开始。

{% hint style="info" %}
为什么是Google引领了大数据技术？
{% endhint %}

Google作为世界上最大的搜索引擎，有着对大规模数据存储和计算的需求，在互联网规模成指数级发展的21世纪，这个需求越来越强烈。另一方面，Google将大数据技术应用在了计算广告领域，广告效果大幅提升，从而给公司带来大量营收，这部分营收又反过来促进Google不断投入到大数据技术的研究当中。在这样的正向激励下，Yahoo、Facebook、Microsoft，Amazon等科技巨头也纷纷加入了大数据领域，促使这项技术得到快速的发展。

{% hint style="info" %}
什么是计算广告？
{% endhint %}
计算广告的目的是在特定语境下找到用户和广告之间的“最佳匹配”，即根据用户搜索的关键词和浏览的网页等信息，推荐给用户对应的广告，并根据用户的点击率持续评估和优化广告效果。可以看到，相比传统广告近乎随机的投放，计算广告可以充分利用大数据技术做到更加精准。因此可以说，在广告领域的成功让大数据技术得到了充足的资源支持。

{% hint style="info" %}
本书你可以学到什么？
{% endhint %}
我们以计算广告中最重要的任务：点击率预估（CTR Prediction）作为背景，阐述大数据技术是如何有效解决这个任务，包括HDFS，MapReduce，Hive，Spark和数据可视化。另外，本书按照大数据技术发展的时间轴设计了众多实验内容，帮助读者循序渐进的了解各项技术的起源，并在实践中理解各项技术的特点，以及这些技术是如何解决点击率预估任务中不同的子任务。最终，本书希望读者可以在完成点击率预估整体任务的同时，对大数据技术有一个全面的了解。

{% hint style="info" %}
本书你学不到什么？
{% endhint %}

本书假定读者已经具备一定的计算机编程基础，全书使用Python作为实验语言，但本书并不是一本Python教程。如果想更好的了解Python编程语言，请读者学习或查阅《Python基础教程》。另外，本书受篇幅所限，并不能对所有大数据技术进行全面讲解。但读者仍可以通过本书的链接到大数据技术对应的官网上进行学习。最后，本书目的在于帮助读者快速上手应用大数据技术解决实际问题，本身并不是一本大数据技术的API手册。鉴于大数据技术发展日新月异，编者强烈建议读者通过技术官网去查阅最新的API文档。




```
GFS：https://static.googleusercontent.com/media/research.google.com/zh-CN//archive/gfs-sosp2003.pdf
MapReduce: https://static.googleusercontent.com/media/research.google.com/zh-CN//archive/mapreduce-osdi04.pdf
BigTable: https://static.googleusercontent.com/media/research.google.com/zh-CN//archive/bigtable-osdi06.pdf
```




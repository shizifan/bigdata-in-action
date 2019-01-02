# Hadoop 架构设计

![](../.gitbook/assets/image%20%282%29.png)

**JobTracker & TaskTracker**

Job Tracker is used to assign MapReduce Tasks to Task Trackers in the Cluster of Nodes. Sometimes, it reassigns same tasks to other Task Trackers as previous Task Trackers are failed or shutdown scenarios.

Job Tracker maintains all the Task Trackers status like Up/running, Failed, Recovered etc.

Task Tracker executes the Tasks which are assigned by Job Tracker and sends the status of those tasks to Job Tracker.


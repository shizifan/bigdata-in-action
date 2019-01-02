---
description: wubin （1）：翻译一下，实验一下，总结一下
---

# 实验五：数据拷贝和分布式拷贝

### cp

```
Usage: hdfs dfs -cp [-f] URI [URI ...] <dest>
Copy files from source to destination. This command allows multiple sources as well in which case the destination must be a directory.
Options:
    The -f option will overwrite the destination if it already exists.
Example:
    hdfs dfs -cp /user/hadoop/file1 /user/hadoop/file2
    hdfs dfs -cp /user/hadoop/file1 /user/hadoop/file2 /user/hadoop/dir
Exit Code:
    Returns 0 on success and -1 on error.
```



### distcp

```
https://hadoop.apache.org/docs/current/hadoop-distcp/DistCp.html
```




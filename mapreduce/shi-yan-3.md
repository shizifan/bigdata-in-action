---
description: wubin（2）：修改一下，试验一下
---

# 实验三：统计特征分布

### 实验描述



### 实验代码

#### mapper**.py**

```text
#!/usr/bin/env python3

import sys
# id,click,hour,C1,banner_pos,site_id,site_domain,site_category,app_id,app_domain,app_category,device_id,device_ip,device_model,device_type,device_conn_type,C14,C15,C16,C17,C18,C19,C20,C21
for line in sys.stdin:
    key = line.strip().split(',')[7]
    value = 1
    print( "%s\t%d" % (key, value) )
```

#### reducer.py

```text
#!/usr/bin/env python3
 
import sys
 
last_key = None
running_total = 0

for input_line in sys.stdin:
   input_line = input_line.strip()
   this_key, value = input_line.split("\t", 1)
   value = int(value)
 
   if last_key == this_key:
       running_total += value
   else:
       if last_key:
           print( "%s\t%d" % (last_key, running_total) )
       running_total = value
       last_key = this_key
 
if last_key == this_key:
   print( "%s\t%d" % (last_key, running_total) )
```

### 单步调试

```text
head -n1000 train.txt | ./mapper.py | sort | ./reducer.py
```

### 作业提交

```text
hadoop \
    jar /opt/cloudera/parcels/CDH-6.1.0-1.cdh6.1.0.p0.770702/lib/hadoop-mapreduce/hadoop-streaming.jar \
    -mapper "python $PWD/mapper.py" \
    -reducer "python $PWD/reducer.py" \
    -input XXXXX \
    -output XXXX
```




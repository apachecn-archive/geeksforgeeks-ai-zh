# 蟒蛇级和熊猫级三角洲。三角洲

> 原文:[https://www . geesforgeks . org/python-pandas-time delta-delta/](https://www.geeksforgeeks.org/python-pandas-timedelta-delta/)

Python 是进行数据分析的优秀语言，主要是因为以数据为中心的 python 包的奇妙生态系统。Pandas 就是其中之一，它让数据的导入和分析变得更加容易。

时间增量是`datetime.timedelta`的一个子类，并且以类似的方式表现。它相当于熊猫的蟒蛇`datetime.timedelta`，在大多数情况下可以互换。`pandas.Timedelta`中的`Timedelta.delta`属性用于返回以纳秒为单位的时间增量。

> **语法:T1】时三角洲。三角洲**
> 
> **参数:**无
> 
> **返回:**返回以纳秒为单位的时间增量

**代码#1:**

```
# importing pandas as pd 
import pandas as pd 

# Create the Timedelta object 
td = pd.Timedelta('3 days 06:05:01.000030') 

# Print the Timedelta object 
print(td) 

print(td.delta)
```

**Output:**

```
3 days 06:05:01.000030
281101000030000

```

**代码#2:**

```
# importing pandas as pd 
import pandas as pd 

# Create the Timedelta object 
td = pd.Timedelta('1 days 7 hours') 

# Print the Timedelta object 
print(td) 

print(td.delta)
```

**Output:**

```
1 days 07:00:00
111600000000000

```

**代码#3:**

```
# importing pandas as pd 
import pandas as pd 
import datetime

# Create the Timedelta object 
td = pd.Timedelta(datetime.timedelta(days = 3, hours = 7, seconds = 8)) 

# Print the Timedelta object 
print(td) 

print(td.delta)
```

**Output:**

```
3 days 07:00:08
284408000000000

```
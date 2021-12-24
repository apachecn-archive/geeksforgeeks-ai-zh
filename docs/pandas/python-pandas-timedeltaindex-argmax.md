# python \ panda 时标索引. argmax

> 哎哎哎:# t0]https://www . geeksforgeeks . org/python 熊猫-timedeltaindex-argmax/

Python 是进行数据分析的优秀语言，主要是因为以数据为中心的 python 包的奇妙生态系统。 ***【熊猫】*** 就是其中一个包，让导入和分析数据变得容易多了。

熊猫 `**TimedeltaIndex.argmax()**`函数返回时间增量索引对象中沿一个轴的最大值的索引。功能类似`numpy.ndarray.argmax`。

> **语法:**时针索引. argmax(轴=None，* args *、* quartz)
> 
> **参数:**
> **轴:**无
> 
> **返回:**整数索引值

**示例#1:** 使用`TimedeltaIndex.argmax()`函数查找给定时间增量索引对象中最大值的索引。

```
# importing pandas as pd
import pandas as pd

# Create the first TimedeltaIndex object
tidx = pd.TimedeltaIndex(start ='1 days 02:00:12.001124', 
                   periods = 5, freq ='N', name ='Koala')

# Print the TimedeltaIndex object
print(tidx)
```

**输出:**
![](img/a3801dc708e61559920bdd986a40bc54.png)

现在我们打印 *tidx* 对象中最大值的索引。

```
# return the index of maximum value.
tidx.argmax()
```

**输出:**
![](img/c4da1af6c2c0cef92db9ffa0e95f2700.png)
正如我们在输出中看到的，`TimedeltaIndex.argmax()`函数有 4，表示 tidx 对象中的最大值出现在第 4 个索引处。

**示例 2:** 使用`TimedeltaIndex.argmax()`函数查找给定时间增量索引对象中最大值的索引。

```
# importing pandas as pd
import pandas as pd

# Create the TimedeltaIndex object
tidx = pd.TimedeltaIndex(data =['-1 days 2 min 3us 10ns', 
                                '1 days 06:05:01.000030',
                                '-1 days + 23:59:59.999999'])

# Print the TimedeltaIndex object
print(tidx)
```

**输出:**
![](img/33758e3fb1552aa13211316292a6719a.png)
现在我们将打印 *tidx* 对象中最大值的索引。

```
# return the index of maximum value.
tidx.argmax()
```

**输出:**
![](img/ce2a2f0ecacdf4a18265d3e02cbc0a1f.png)
正如我们在输出中看到的，`TimedeltaIndex.argmax()`函数的值为 1，表示 tidx 对象中的最大值出现在第一个索引处。
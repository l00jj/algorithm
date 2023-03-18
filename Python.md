使用defaultdict修改默认行为
```python
dic = defaultdict(int)
dic[0] += 1
dic[-1] = 1
```
```python
import bisect
# 二分查找,_right下标 + 1
bisect(arr, target)
bisect_right(arr, target)
# 二分插入函数
bisect.insort()
```
### 函数如何引入比较器
```python
import operator
operator.add
operator.xor
```
### 如何定义参数和使用
(num=123,val) 报错，带默认值的参数必须放在最后
(val,\*,num=123)这个\*用于隔断之前的值，如果要修改最后num的值，需要在使用的时候fun(1,num=7)这样修改

[参考](https://www.cnblogs.com/happyyangyanghappy/p/17085375.html)

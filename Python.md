### 倒序对比
`a == a[::-1]`，字符串头部与结尾双指针对比，常用于回文判断
### 使用defaultdict修改默认行为
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
### 叠加器/累加器
```python
# http://study.yali.edu.cn/pythonhelp/library/itertools.html#itertools.accumulate
itertools.accumulate(iterable[, func, *, initial=None])
[v for v in enumerate(accumulate(list, operator.mul))]
# http://study.yali.edu.cn/pythonhelp/library/functools.html?highlight=reduce#functools.reduce
functools.reduce(function, iterable[, initializer])
```
### 如何定义参数和使用
(num=123,val) 报错，带默认值的参数必须放在最后
(val,\*,num=123)这个\*用于隔断之前的值，如果要修改最后num的值，需要在使用的时候fun(1,num=7)这样修改

https://www.cnblogs.com/happyyangyanghappy/p/17085375.html

### 优先堆的使用
它主要的特点是需要一个额外的数列，并且原地修改这个数列，如果是pop这种弹出操作，数列会真实减少长度
http://study.yali.edu.cn/pythonhelp/library/heapq.html

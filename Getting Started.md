# TensorFlow入门、基本用法

## 导入

```
import tensorflow as tf
```

使用CPU的可以用下面的，不然会报一堆错误

```
import os
os.environ['TF_CPP_MIN_LOG_LEVEL']='2'
import tensorflow as tf
```

## 初始化tensorFlow runtime

```
sess = tf.Session()
```

## tensor加减

```
node1 = tf.constant(3.0, dtype=tf.float32)
node2 = tf.constant(4.0)
print(sess.run(a+b))
```

可以看到结果7了

## placeholder

```
a = tf.placeholder(tf.float32)
b = tf.placeholder(tf.float32)
plus = a * b
r = sess.run(plus,{a:[1.2,2.2], b:2})
print(r)
```

类似一个函数，上面是二维向量乘以一个一维向量，结果是`[ 2.4000001  4.4000001]`


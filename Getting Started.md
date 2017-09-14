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


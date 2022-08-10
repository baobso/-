# lgb参数

**数据转换**

![image-20220810142709404](C:\Users\bao\AppData\Roaming\Typora\typora-user-images\image-20220810142709404.png)





**num_boost_round** :建立多少树

**valid_sets** ,评估的数据,以[]的形式存储,可以同时存储 训练的数据 和评估的数据

![image-20220810142130338](C:\Users\bao\AppData\Roaming\Typora\typora-user-images\image-20220810142130338.png)

**valid_names** ,和**valid_sets** 一样使用,把名字改了,没啥用其实

**categorical_feature**:lgb会对cat类型的数据另外处理,可以以列表的形式写下去

```python
tr1['goods_id']=tr1['goods_id'].astype('category')

```

类别需要转换

**early_stopping_rounds**:多少轮没有提升,停止迭代

**evals_result**: 传入一个空字典就可以了,会存放evals评估的数据

![image-20220810142551417](C:\Users\bao\AppData\Roaming\Typora\typora-user-images\image-20220810142551417.png)

![image-20220810142600567](C:\Users\bao\AppData\Roaming\Typora\typora-user-images\image-20220810142600567.png)

# xgb参数


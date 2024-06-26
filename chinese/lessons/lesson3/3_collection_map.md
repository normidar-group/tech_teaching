# Map(或者说Dictionary)

Map是一种更灵活的集合，它可以自己定义索引，而不像List那样只能用数字索引。Map的索引称为键(Key)。

废话不多说，直接看例子：

```dart
Map<String, String> mm = {
  'name': 'normidar',
  'age': '18',
};
print(mm);
```

观察一下代码，看看发现了什么。（和上一节的List的用法比较一下）


## 键值对 (Key Value)

这就要讲到数据的理想形态了，其实键值对是非常之多功能又自由的一种数据形式，它是二维数据的理想形态。


想象一下，如果要把全世界的人装入一个数据库，我们应该怎么装呢？

常用的解决方案是这样的：


| name | age | sex | address | phone |
| ---- | --- | --- | ------- | ----- |
| Normidar | 18 | male | Japan | 123456789 |
| Jerry | 20 | female | UK | 987654321 |
| Tom | 15 | male | USA | 123123123 |
| Jack | 30 | female | China | 456456456 |
| ... | ... | ... | ... | ... |

这样的表格，就是数据库的形式，而把其中一行的数据取出来我们就可以得到一个Map。

```dart
Map<String, String> lowMan = {
  'name': 'normidar',
  'age': '18',
  'sex': 'male',
  'address': 'Japan',
  'phone': '123456789',
};
```

哈哈，理解了吗？

在数据库中、「name」「age」「sex」「address」「phone」这些列名叫做Field（叫什么不重要，重要要理解它是什么），而对应到Map时它们就是Key（键）。

先写到这里，明天继续写Map的用法，但基本和List是差不多的。

---

好，回到正常的教程。

Map是数据储存的类型，那他就有增删改查。

## 增加

```dart
Map<String, String> mm = {
  'name': 'normidar',
  'age': '18',
};

mm['sex'] = 'male'; // 增加一个键值对(因为`sex`这个键不存在)
print(mm);
```

## 删除

```dart
Map<String, String> mm = {
  'name': 'normidar',
  'age': '18',
};
mm.remove('age'); // 删除键值对
print(mm);
```

## 修改

```dart
Map<String, String> mm = {
  'name': 'normidar',
  'age': '18',
};
mm['age'] = '19'; // 修改键值对(因为`age`这个键存在所以会执行修改)
print(mm);
```

## 查找

```dart
Map<String, String> mm = {
  'name': 'normidar',
  'age': '18',
};
print(mm['name']); // 直接打印键对应的值
print(mm['gggg']); // 如果键不存在则返回null (Dart不会报错, 但是在其他语言中可能会报错)
```


OK, 今天就写到这里，我看看我写了什么内容然后下一课写写练习题。
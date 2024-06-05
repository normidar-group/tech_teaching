
# Literal リテラル　字面量

按照四个基础类型，Literal也分四种：

- String -> 使用双引号引住text就是String的Literal
  - 缩写是str
- Integer -> 整数直接写上
  - 缩写是int
- Float or Double -> 小数直接写上
  - 没有缩写
- Boolean -> 写true或者false
  - 缩写是bool

## 例子

- "abc" -> 属于String
- 1 -> 属于Integer
- 2.5 -> 属于Float/Double
  - 2.0 -> 这样的也属于Float/Double
- true -> 属于Boolean
- false -> 属于Boolean

# Calculate 计算

计算也分为4种计算：

- 四则（+-*/）
- 比较（>, <, >=, <=, !=, ==）
- 逻辑（or, and, not）
- 字符串连接（+）

每种计算方法有不同的输入类型和输出类型，下面逐一介绍：


## 四则运算

和数学一样，它是对数进行运算：

- 输入：数（Integer or Float/Double）
- 输出：数（Integer or Float/Double）

例子：

- 1 + 1  (int to int)
- 2 * 3  (int to int)
- 9 / 2  (int to float)
- 2.0 - 0.5 (float to float)

## Compare 比较

比较运算的输入是数，输出是Boolean。

例如：

- 3 > 2 的结果是 true
- 2 == 3 的结果是 false (因为2不等于三) == 是判断是否相等的符号
- 2 != 3 的结果是 true (因为2不等于三) != 是判断是否不等的符号
- 4 >= 4 的结果是 true (因为4大于等于4) >= 是大于等于的符号
- 6 <= 7 的结果是 true (因为6小于等于7) <= 是小于等于的符号
- 2 <= 1 的结果是 false (因为2不小于等于1)

## logic 逻辑

逻辑运算的输入是Boolean，输出也是Boolean。

最常用的是`or, and, not` 这三种运算。

### OR 或者

两边只要有一个是true就计算出true， 运算符是 ||

- true || true 结果是 true
- true || false 结果是 true
- false || true 结果是 true
- false || false 结果是 false

| OR | T | F |
|----|---|---|
| T  | T | T |
| F  | T | F |

### AND 并且

当两边是true时返回true, 否则返回false，运算符是 &&

- true && true 结果是 true
- true && false 结果是 false
- false && true 结果是 false
- false && false 结果是 false

| AND | T | F |
|-----|---|---|
| T   | T | F |
| F   | F | F |

### NOT 取反

取Boolean相反的值，运算符是!

- !true 结果是 false
- !false 结果是 true

## 字符串连接

将两边的字符串连接起来, 输入是String输出也是String。

- "A" + "B" 结果是 "AB"

> 这里补充一下：`+`号在四则运算中是加法运算符，而在字符串连接中是连接符。这里虽然是同一个符号，但是因为输入的类型不同，功能也不同。


## 扩展（可以跳过）

在加密计算领域（例如密码，银行系统，文件加密等应用场景）还有一个比较常用的逻辑计算，叫做「异或」运算（XOR）。平时打代码完全不会用到这个运算，但是在加密领域是比较基本的运算。

它是这样的：相同为false，不同为true：

- true xor true 结果是 false
- true xor false 结果是 true
- false xor true 结果是 true
- false xor false 结果是 false

| XOR | T | F |
|-----|---|---|
| T   | F | T |
| F   | T | F |

Q：那么它为什么可以用在加密上呢？

这个问题问得好，请看下面的例子：

我们知道，计算机中的数据都是以二进制的形式存储的，true和false一一对应1和0。那么我们可以用XOR运算来加密数据：

有一个数据是这样的：`1010`，我们想要加密它，我们有一个密钥是`1100`，我们可以用XOR运算来加密：

```
1010 xor 1100 = 0110
```

这样我们获得了一个加密后的数据`0110`。

好，请把密匙收在裤袋，把原始数据`1010`忘掉（删除掉）。


有一天，我想要解密我的`0110`，这时请从裤袋里拿出密匙`1100`，再次进行XOR运算：

```
0110 xor 1100 = 1010
 ↑         ↑      ↑
加密数据   密匙   解密后得到的数据
```

嚯嚯，神不神奇？


## 尝试一下

请问下面的计算结果是多少？

- 1 + 1
- "3" + "4"
- true || false
- false && true
- 4 > 3
- 3 == 3
- 3 != 3
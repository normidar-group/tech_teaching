
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

和数学一样，它通常是对数进行运算：

- 输入：数（Integer or Float/Double）
- 输出：数（Integer or Float/Double）

例子：

- 1 + 1  (int to int)
- 2 * 3  (int to int)
- 9 / 2  (int to float)
- 2.0 - 0.5 (float to float)

思考题：`float to int` 有可能吗？

## Compare 比较

比较运算的输入是数，输出是Boolean。

例如：

- 3 > 2 结果是 true
- 2 == 3 结果是 false (因为2不等于三)
- 2 != 3 结果是 true
- 4 >= 4 结果是 true
- 6 <= 7 结果是 true
- 2 <= 1 结果是 false

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
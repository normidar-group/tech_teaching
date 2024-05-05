
# 进入代码的世界


进入代码的世界最后会了解到几个基本的概念，希望读者在能在学完所有后检查自己是否理解以下几个概念，但在一开始不会全部讲解（现在看不懂完全没问题，当作记下英语单词）：

- Statement -> 语句
- Expression -> 表达式
- Type -> 类型
  - Generic -> 泛类型
- Literal -> 字面量
- Branch -> 分支
- Loop -> 循环

在更深入时，希望能理解(现在看不懂没关系，頭の片隅に置いて大丈夫です)：

- Class -> 类
- Extends -> 继承
- Abstract -> 抽象
- Implements -> 实现
- Overrides -> 覆盖

## 最最基础的概念


- Expression(式 (读作しき)) -> 表达式
  - 会获得某个值的东西（额，好难解释。。）
  - 有很多东西是归于`表达式`这类的，慢慢去感觉它是什么
  - 表达式说获得的值会属于某些类型，例如 `1 + 1` 这个表达式是属于整数类型的（因为整数相加总是等于整数）
- 计算（计算是一种表达式(Expression)因为它会获得某个值）
  - 计算通常有以下几种
    - 四则
    - 比较
    - 逻辑（or, and, not）
    - 字符连接
- BaseType -> 基础类型
  - 一般有四个基本类型：
    - String -> 字符串
    - Integer -> 整数
    - Float or Double -> 带小数点的数（叫精数）
    - Boolean -> 布尔值（只可以储存true和false的计算机里的最便宜的数据类型，因为计算机是用0,1来储存数据的）
- Literal(リテラル) -> 字面量 (字面量也属于表达式，因为它就是某个值)
  - 写死在代码中的数据
  - 每个基础类型都有对应的字面量的记述方法


## Dart语言

其实哪个语言背后的原理是一样的，熟悉一个就能熟悉多个。

先讲我最常用的Dart。

Dart来源于Java，很多Java语法Dart都通用，但Dart更多功能在某些情况能更方便地构建想要的逻辑。

[Dart可以在线执行，试用它的功能。](https://dartpad.dev/)

## Hello World

由于来自Java它不像Python,JS等可以无入口执行，它必须要有main(){}这样的入口函数来进入逻辑。（关于函数会在以后讲）

尝试以下代码：

```dart
void main() {
    print("Hello World!");
}
```

其中`"Hello World!"`就属于String的Literal.

而`print`会将其后面括号里的表达式的值输出到Command Line.







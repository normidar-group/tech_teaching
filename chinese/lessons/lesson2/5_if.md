# 分支 Branch

什么是分支？

分支指的是在程序中根据某些条件而执行不同的代码（条件是condition, 代码我们用code来表示）

这里的分支英文是Branch，但这里不使用英语，因为Branch通常指的是另一样东西（Git branch）

首先讲解的是IF.

## IF

- if
- else
- eles if

由于Dart和Python都比较难看清楚，尝试使用Swift来说明一下（相对`Dart`它的`condition`周围不用小括号，相对Python它更接近程序员使用的语言）：

if的格式

```swift
if condition {
    code
} else if condition {
    code
} else {
    code
}
```

### Condition

`Condition`的意思是条件，`if`和`else if`后都要接`Condition`.

`Condition`中放的必须是`Boolean`的表达式。

当且仅当`Condition`中的值为`true`时它对应的`Statements`才会执行，

### Statements

现在可以暂时理解为代码，可以放零行以上的代码在`{}` 中。

### 其它的规则

- `if...`必须放在最前面 (`else if`或者`else`不能放在最前面)
- `else if`的个数可以是零或以上
- `else`的个数可以是零个或者一个

### 例子

只有`if`时（`else if`和`else`的个数都是零个）：

```swift
if 3 > 0 {
    print("3 bigger than 0")
}
```

有`if`和`else`时：

```swift
if 3 > 0 {
    print("3 bigger than 0")
} else {
    print("3 smaller or equal to 0")
}
```

全部都有时：

```swift
if 3 > 0 {
    print("3 bigger than 0")
} else if 3 < 0 {
    print("3 smaller than 0")
} else {
    print("3 equal to 0")
}
```


只有`if`和`else if`也可以的：

```swift
if 3 > 0 {
    print("3 bigger than 0")
} else if 3 < 0 {
    print("3 smaller than 0")
}
```

## 重点

由`if`, `else if` `else`组成的分支组中最多只能执行一个分支(有不被执行的情况)，但如果有`else`存在则必然有一个分支被执行，因为`else`是前面的条件都不通过时`else`就会被执行。
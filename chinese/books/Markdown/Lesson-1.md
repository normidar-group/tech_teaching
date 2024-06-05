
# Markdown 程序员的写作格式

> Markdown的功能是使用一些简单的符号来制作一个简单又比较可观的文章，它是程序员的一个基本技能。

当创建文本来供给别人阅读时，如果使用txt文件，那将会变得难以阅读。<br>
而如果使用word文档，那将变得难以更改（你必须下载微软他家的软件然后双击再等几秒）<br>
Markdown就是这两个难题的一个解决方案

如果你想尝试美丽的Markdown，你可以试下这些软件：https://notepm.jp/blog/724 ,但我会在后面会介绍一个非常常用的软件：VSCode。

以下介绍Markdown的各个功能的格式和其用法：

## 具体的使用方法

### 创建标题 -> `#`

格式：

`# 标题`

展现的效果如下：

# 标题


格式是`#`号加空格加你想写的标题，`#`号的个数是1个到6个，个数越多标题的级别越低：

例如：

- `## 标题` -> 这是二级标题或者叫副标题
- `### 标题` -> 这是三级标题或叫副副标题
- 如此类推

### 罗列 -> `-`

格式：

> `-`加空格加内容，想缩进时加两个以上的空格到左边。
> 缩进的目的是表达从属关系。

例如：

```
- Apple
   - Green Apple
   - Red Apple
- Orange
- Banana
```

展现的效果如下：

- Apple
   - Green Apple
   - Red Apple
- Orange
- Banana

### 有序罗列 -> `1.`

> 原理和罗列一样

格式：

```
1. Apple
   1. Green Apple
   2. Red Apple
2. Orange
3. Banana
```

效果

1. Apple
   1. Green Apple
   2. Red Apple
2. Orange
3. Banana

### 换行 -> `<br>`

> 在Markdown中换行需要使用来自HTML的`<br>`, 由于效果无法展示请自己尝试效果。（Markdown是HTML的扩展包，所以在HTML上可以用的东西都可以在Markdown上使用）

### 超链接 -> `[...](...)`

格式：

```
[你想展示的文字](你要跳转的页面)
```

例如：

```
[跳到谷歌](https://google.com/)
```

效果:

[跳到谷歌](https://google.com/)

### 引用 -> `>`

当我们需要引用某人讲的话，或者讲一句又短又精髓的话时，我们会使用"引用"。

格式：`>`加空格加内容

例如:

```
> 床前明月光，疑是地上霜。
```

效果：

> 床前明月光，疑是地上霜。

### 小片段 -> ``

例如：

```
学习用`Markdown`来写作
```

效果：

学习用`Markdown`来写作

### 多行片段（代码片段） -> ``````

格式：

上面放三个```下面也放三个

例如(为了易于展示，我加入了空格，实际是不用空格的)：

```
` ` `
My codes
` ` `
```

效果:

```
My codes
```

## 补充知识

> Markdown是HTML的扩展, 所以所有HTML的Tag都可以在Markdown中使用。

> 根据渲染器的不同，Markdown的展现方式会有所不同，不用太在意这些微小的不同

> 可以看看[菜鸟教程](https://www.runoob.com/markdown/md-title.html)去了解更多其它功能



## 练习

尝试制作出以下效果的页面：

![](/images/markdown_training.png)

## 作业

使用Markdown写一篇笔记（要用到至少3个符号）


## 课后思考

> (注：课后思考通常是与知识无太大关系的东西，看不明就算了)

#### 什么是渲染？ (Rendering)

我以前在职中学过关于3D建模的相关知识，对“渲染”这个词有个人的见解。

在谷歌中你可能会查到如下的解释：

> 使用艺术来表现事物的过程。

我会这样解释这个词：

> 从数据到可视化的过程（数据可视化的行为）

在3D建模中它是计算“光线”，“材质”，“形状”的过程。

在Markdown中它是对文字进行展示。


> 额，回头Check下这段，我也不知道我在写什么，哈哈😄
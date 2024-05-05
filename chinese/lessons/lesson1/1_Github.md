# Github: 程序员的身份证

Github有很多的用途，简单来理解的话可以理解成用来储存代码在网上的工具，它使用Git的技术来储存代码。（将会在后面的课程中介绍Git的使用）

Github账号同时是一个程序员的身份证，你可以在上面储存你的代码，你的项目，你可以公开自己的代码也可以去看看学习别人的代码。

## 创建GitHub账号

能看到我这篇文章的人已经是创建了GitHub账号的了，创建方法就不写了

## 基本概念

### 用户名

用户名通常是一串字母，中间也可以夹杂一些数字和符号，Github的用户名是全球唯一的，如果某人创建了某个用户名其他人将无法创建。

例如我的用户名是`normidar`其他人将无法使用此名称作为Github的用户名，这相当于程序员的一个身份证。（特别是开源项目的程序员）

### 个人页面

个人页面的格式是这样的：

`github.com/用户名`

例如我的个人页面是这样的：

[github.com/normidar](https://github.com/normidar)

### Repository

Repository中文叫仓库，是储存整个项目代码的地方，按照以下步骤来创建Repository：


1. 进入自己的个人页面
2. 点击`Repository`：
    1.  ![](/images/github_reposi.png)
3. 点击`New`：
   1. ![](/images/github_new_repo.png)
4. 填写`Repository name`
   1. ![](/images/github_repo_name.png)
5. 选择`Private`（如果你想公开你的代码，可以选择`Public`）
   1. ![](/images/github_choose_private.png)
6. 点击`Create repository`
   1. ![](/images/github_create_repo.png)

这样你就创建了一个你的`Repository`。

#### 说明：

Repository的网页地址总是：github.com/用户名/Repository名

例如这篇文章的网页地址是：[github.com/normidar/tech_teaching](https://github.com/normidar/tech_teaching)

### Issue

什么是Issue?

Issue 的中文直译是「问题」，如果不出意外代码会是不够完善的，或者存在Bug的，这时候我们可以修正它，或者创建Issue以后来做到：

- 以后修正代码
- 叫其他人修正这代码

总之，Issue是作为一个备忘录一样的存在。（Issue是在Repository里面的，它不能独立存在）

#### 创建Issue

以下方法来在Repository上创建Issue:

1. 进入Repository的主页
2. 点击`Issue`
   1. ![](/images/github_issue.png)
3. 点击`New issue`
   1. ![](/images/github_new_issue.png)
4. 填写标题和说明文
   1. ![](/images/github_write_issue.png)
5. 点击`Submit new issue`来提交新的Issue
   1. ![](/images/github_submit_new_issue.png)

#### 查看Issue

创建Issue后你会发现`Issue`按钮右边会有数字变化：

![](/images/github_issue_count.png)

点击它就可以查看现有的Issues

#### 关闭Issue

不建议删除Issue，建议关闭Issue:

在Issue的页面中点击`Close issue`来关闭Issue:

![](/images/github_close_issue.png)


## 总结

这篇教程写了Github中的两个概念：Repository和Issue，Repository是用来储存整个项目的，Issue则是用于指出项目中的问题以备往后修正以及讨论。

## 练习

1. 创建repository
2. 创建issue
3. 关闭issue


## 课后思考

> (注：课后思考通常是与知识无太大关系的东西，看不明就算了)

#### 状态的变化与状态

> Q：事物的如今状态是怎样来的？
>
> 思考：是由过去的「状态的变化」“堆积”而来的。
>
> 请举个例子
>
> 思考：比如我一开始身无分文，我的钱包的状态是0元。一日，我赚了10元，我的钱包的状态就变成了10元。我又花掉5元，我的钱包的状态就是5元。这样，钱的变化就是「状态的变化」，只要我们记录了所有的「状态的变化」我们就可以推算出现在的状态。
>
> 与这课的关系？
>
> 思考：Github的核心是一个版本管理器叫Git，虽然还未讲到Git，但Git的思想就是记录「状态的变化」来推算出如今状态的。
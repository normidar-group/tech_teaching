# 命令 Command

这里讲的命令是Linux的一些基础的命令，下面讲到Command时指的就是命令。

## 终端 Terminal

终端是指执行命令的地方，通常服务器是没有图形界面的，所以我们在连接服务器时做的所有行为都是在终端上执行Command，在下面讲到Terminal都是指终端。

## 打开Terminal

在MacOS上要打开Terminal，可以按`command + space`然后输入`Terminal`再按回车来打开。（注：MacOS是Linux类似的系统，所以大部分Linux的Command都可以在MacOS上运行）

也可以在应用中查找叫`Terminal`的软件然后打开它。

软件的图标：

![](/images/terminal_icon.png)

打开后的界面（可能和你的会有些小差异）：

![](/images/terminal_image.png)

> 如果你使用的是Windows系统，你可以尝试了解下PowerShell，它是类似的东西。（不过使用Windows的服务器很少，实在没有机器可以先跳过本章）

### 在MacOS中快捷地打开Terminal

进入Finder(中文叫`访达`)，在下方的地址栏中右键某目录，弹出来的菜单中选择「在终端打开」。

![](/images/finder_bottom_bar.png)

![](/images/finder_bottom_right_click.png)

## 界面介绍

在打开Terminal之后你会见到如下的一行文本(其它行都是不重要的， 重要的只是这一行)：

![](/images/terminal_command_line.png)

中间会有一个`%`(有时候它会是`$`号)不过都无关紧要，这个符号的右边是用来输入Command的，左边是显示用户名和当前目录的。（目录又叫文件夹，directory或folder都是指代它）


# 常用的Command

> 在输入完Command之后按`回车键`执行该Command

## 查看此目录下的内容： `ls`

语法：ls （嗯，就两个字母）

具体效果：

![](/images/command_ls.png)

## 更改目录： `cd`

使用cd来更改目录，语法是`cd [你的目录]`（`cd` 是 Change Directory 的简写）

按回车之后`%`的左边所显示的目录会发生改变。

1. 切换到当前用户的主目录：
  - cd ~
2. 切换到上级目录：
  - cd .. 
3. 切换到根目录：
  - cd /
4. 切换到某个具体的子目录：
  - cd mulu

## 创建文件夹： `mkdir`

格式：

```
mkdir 你要创建的文件夹名
```

## 创建空白的文件： `touch`

格式：

```
touch 你要创建的文件名
```

## 删除文件或文件夹： `rm -rf`

格式：

```
rm -rf 你要删除的文件或文件夹名
```

## 显示文本文件的内容： `cat`

格式：

```
cat 要显示的文件名
```



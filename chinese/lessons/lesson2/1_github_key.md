# 不懂时谷歌， 只示范一下 （不太常用而且难记忆）

可以参考下：https://docs.github.com/zh/authentication/connecting-to-github-with-ssh/adding-a-new-ssh-key-to-your-github-account

## 目的

将本地的`terminal`连接到Github以获得Github仓库的操作权。



---


用GPT生成了下（仅供参考）：


## 目的

通过在本地终端上配置SSH密钥，实现与GitHub仓库的安全连接，从而获得对GitHub仓库的操作权限。

## 步骤

1. **生成新的SSH密钥：** 

   在本地终端上执行以下命令来生成新的SSH密钥：

   ```bash
   ssh-keygen -t rsa -b 4096 -C "your_email@example.com"
   ```

   替换`your_email@example.com`为你的GitHub注册邮箱。

2. **将SSH密钥添加到SSH代理：**

   如果你尚未启动SSH代理，则可以使用以下命令启动：

   ```bash
   eval "$(ssh-agent -s)"
   ```

   然后，将SSH密钥添加到SSH代理：

   ```bash
   ssh-add ~/.ssh/id_rsa
   ```

   如果你使用的不是默认的SSH密钥文件名，请相应地替换`~/.ssh/id_rsa`。

3. **将SSH密钥添加到GitHub帐户：**

   复制你的SSH密钥到剪贴板：

   ```bash
   pbcopy < ~/.ssh/id_rsa.pub
   ```

   然后，前往GitHub网站，登录你的帐户，转到“Settings” > “SSH and GPG keys”，点击“New SSH key”，将剪贴板中的SSH密钥粘贴到“Key”字段中，然后点击“Add SSH key”。

   注意：如果你的系统不支持`pbcopy`命令，你可以手动打开`id_rsa.pub`文件，并复制其中的内容。

4. **测试SSH连接：**

   在终端中执行以下命令来测试SSH连接是否成功：

   ```bash
   ssh -T git@github.com
   ```

   如果一切正常，你应该会收到一条消息，确认你已成功连接到GitHub。

通过按照以上步骤配置SSH密钥，你将能够安全地连接到GitHub仓库并进行操作。

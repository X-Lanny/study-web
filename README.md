# 关于学习历程、笔记 或者 心得

## git/终端 语法等
1. git push -u origin master”
>error: src refspec master does not match any
>error: failed to push some refs to 'github.com:xxxxx/firsthub.git' 
>这个错误通常表示本地的 master 分支可能为空或不存在。
>根据github上提供的语法看一下分支名称，直接贴过去 "> 的效果"

2. github仓库页面可以切换https / git
3. SSH 连接到远程仓库时的首次连接询问，通常会在第一次连接时出现。Git 在首次连接时会询问你是否信任远程主机的身份验证信息。
4. git add .*(有空格)* 
>git commit -m 'word peace'  
>git push
5. cd /xxxx *（前面空格后面没有空格）*
6. 关于文件夹位置的关系，有些时候报错可以退回到cd 再进来
7. (在终端中) cat 命令用于打印文件内容，文件存在就会在终端打印出文件内容，不存在则会提示没有这个文件。

## 名词解释
1. **Markdown** 是一种轻量级标记语言，使用易读易写的纯文本格式编写文档
2. **git** Git 是类似 CSV 或 SVN 的代码版本管理工具
3. **CSV** 
4. **SVN** 
3. **http**  HTTP（Hypertext Transfer Protocol）是一种用于传输超文本的应用层协议。它是互联网上用于在网络浏览器和 Web 服务器之间传递文本、图像、音频、视频以及其他多媒体文件的基础协议。
4. **ssh** SSH Key（Secure Shell Key）是一种用于安全访问远程服务器的身份验证方法。SSH（Secure Shell）是一种加密的网络协议，用于在网络中安全地传输数据。SSH Key 是一对密钥，包括私钥和公钥，用于身份验证和加密通信。
5. **.md** Markdown 文件格式使用 .md 后缀


## 有趣的关联性
1. heading 使用“#“的含义和notion、飞书相同；
    - ![notion image](https://upload.wikimedia.org/wikipedia/commons/thumb/e/e9/Notion-logo.svg/200px-Notion-logo.svg.png ) *绝对路径*
    - ！[feishu image](./upload.wikimedia.org/wikipedia/commons/thumb/4/42/Lark_Suite_logo_2022.png/440px-Lark_Suite_logo_2022.png)*相对路径????*     **可能不是这样，但案例里的图片导入github也无法显示**
    - [notion](https://www.notion.so/)
    - [feishu](https://www.larksuite.com/en_us?from_site=feishu)
2. 斜体、加粗语法和notion相同，和飞书大概也相同；

## 问题
1. "使用![]()" 这里应该使用谁的相对路径？我吧http删掉了，但图片并无法显示出来，下图案例也无法显示出来。
    - ![使用相对路径](./images/markdown-image.jpeg)
2. 关于github page 的问题；虽然成功创建出来了，但并非是文档中的方法：
    - [创建成功的URL](https://x-lanny.github.io/ )
    - [使用方法为知乎找到的](https://zhuanlan.zhihu.com/p/91652100)
使用文档中的方法：
到最后一步
    >“git push -u origin master” (对我的GitHub来说位置是main,所以后面的代码都是main)
    > 终端要求输入用户名和密码；
    > 但无法输入密码，原因是粘贴不上去；
    > 问了gpt，它表示“在终端中输入密码时，通常是不会显示密码字符的，这是出于安全考虑。即使你输入密码时看不到字符，实际上系统仍在接受你的输入。
    > 当你按下回车键时，如果密码正确，系统会继续执行相应的命令。如果密码错误或其他问题，系统可能会显示错误消息。”
    > 于是我粘贴了，出现了一下的结果：
    > lancer_x@xxMacBook-Pro ~ % cd /Users/lancer_x/Desktop/X-Lanny.github.io
    > lancer_x@xxMacBook-Pro X-Lanny.github.io % git init
    > Initialized empty Git repository in /Users/lancer_x/Desktop/X-Lanny.github.io/.git/
    > lancer_x@xxMacBook-Pro X-Lanny.github.io % git add .
    > lancer_x@xxMacBook-Pro X-Lanny.github.io % git commit -m "first commit"
    > [main (root-commit) d299709] first commit
    >  1 file changed, 1 insertion(+)
    >  create mode 100644 index.html
    > lancer_x@xxMacBook-Pro X-Lanny.github.io % git remote add origin https://github.com/X-Lanny/X-Lanny.github.io.git
    > lancer_x@xxMacBook-Pro X-Lanny.github.io % git push -u origin main *从这里开始，失败了*
    > Username for 'https://github.com': X-Lanny
    > Password for 'https://X-Lanny@github.com': 
    > remote: Invalid username or password.
    > fatal: Authentication failed for 'https://github.com/X-Lanny/X-Lanny.github.io.git/'
    > lancer_x@xxMacBook-Pro X-Lanny.github.io % 



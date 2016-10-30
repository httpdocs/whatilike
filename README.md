# whatilike
##一个自己写的喜欢的网站的导航页，里面是一些自己常用的网站，主要是编程和设计类的网址居多，供自己学习和浏览方便。

# 首文打算记录我是如何制作我的第一个github主页

- [ ] 首先是注册github账号，下载github客户端和git版本控制工具。


- [ ] 然后，新建了一个repository，点击自定义的仓库名称进入仓库，点击Setting，只需在里面再点击Launch automatic page generator，选个主题便可。

- [ ] 我们要在本地创建一个gh-pages分支，因为GitHub隐藏的建立了一个gh-pages分支，这个分支你在客户端看不到，可以在网页版看到。为了方便我们让这个分支在客户端也能看到。这个分支规定保存网页所有源文件。

- [ ] 在创建gh-pages分支之前，我们先测试一下，打开git-bash，输入下面的命令，看看设置是否成功，`git@github.com`的部分不要修改：

      ```
      $ ssh -T git@github.com 
      ```

- [ ] 如果是下面的反应：

      C代码  

      ```
      1.The authenticity of host 'github.com (207.97.227.239)' can't be established.  
      2.RSA key fingerprint is 16:27:ac:a5:76:28:2d:36:63:1b:56:4d:eb:df:a6:48.  
      3. Are you sure you want to continue connecting (yes/no)?  
      ```

      不要紧张，输入`yes`就好，然后会看到：

      C代码 

      ```
      1.Hi <em>username</em>! You've successfully authenticated,
      but GitHub does not provide shell access.  
      ```

      一切正常。

- [ ] 设置账户信息。现在你已经可以通过SSH链接到GitHub了，还有一些个人信息需要完善的。Git会根据用户的名字和邮箱来记录提交。GitHub也是用这些信息来做权限的处理，输入下面的代码进行个人信息的设置，把名称和邮箱替换成你自己的，名字必须是你的真名，而不是GitHub的昵称。

      ```
      $ git config --global user.name "你的名字"  
      $ git config --global user.email "your_email@youremail.com"  
      ```


- [ ] 先创建一个同名的gh-pages，这时这个分支才会在你的客户端和本地文件夹中显示。

      ```
      cd 你的根目录名字
      ```

      初始化一下,创建目录。

      ```
      $git init
      $ git checkout --orphan gh-pages
      ```

------

**期间借鉴的文章有：**

- http://www.ruanyifeng.com/blog/2012/08/blogging_with_jekyll.html
- http://justcoding.iteye.com/blog/1959737
- http://blog.csdn.net/apolo_/article/details/51167180
- http://www.jianshu.com/p/31cbbbc5f9fa/

# git_learning-using_demo

## 学习git

![image-20220705221656504](https://img2022.cnblogs.com/blog/2737817/202207/2737817-20220706232120722-1365924680.png)

> 这个文档是`git`的入门使用文档

- [Learn Git Branching](https://learngitbranching.js.org/?demo=&locale=zh_CN)
- 还有B站的一堆教学视频就不一一列举了，资源非常多；
- 学完上面那个可以直接实操一下[【狂神说Java】Git最新教程通俗易懂_哔哩哔哩_bilibili](https://www.bilibili.com/video/BV1FE411P7B3?p=14&vd_source=ee7084e0c5101ce0d8d076550c3bc93c)

> 上面那个B站的视频系列看最后几讲P8~P14完全够用了，而且它那个配置是2020年的`gitee`，本人用的是`github`，但里面对分支的还是没有很清晰，主要是给想去大厂工作的同学需要。

下面是自己总结的一些实用功能；

## 上传步骤（在命令行中操作）

1. 打开有`.git`的文件夹，右键`git bash`字样的东西；
1. `git add .`把当前目录下的所有文件`add`到那个`.git`（版本库）中的`index`（暂存区）去;
2. `git commit -m 'some data'`后面的更新的信息一定要自己写上去，不然会自动打开`Vim`让你写（写完下方 输入`:wq`退出）
3. `git push`即可；

![image-20220705235003412](https://img2022.cnblogs.com/blog/2737817/202207/2737817-20220706232120168-1314930032.png)

### 额外知识补充：

现在很多人是使用图形化操作界面来`push`的，比如`IDEA`（上面那个B站视频有）来直接`commit`等等操作，还有这个是使用`SourceTree`的[使用SourceTree - 廖雪峰的官方网站 (liaoxuefeng.com)](https://www.liaoxuefeng.com/wiki/896043488029600/1317161920364578)

目前暂时也没有修改一堆分支的需求也没有用到`IDEA`的，感觉命令行是最简洁的，但分支的基本操作确实是在那个游戏一样的教程里面很全面了：更多的学习可以看这个[Git教程 - 廖雪峰的官方网站 (liaoxuefeng.com)](https://www.liaoxuefeng.com/wiki/896043488029600)

----

<center>2022.7.6来更新一下</center>

> `github`自己设置公共仓库上传的单个文件不能超过100MB，这也就决定了如果有大的压缩包，又比如某些文件的安装包想留个备份都不太适合，在报错时给出了其它的储存大文件的`git`网站，没细了解，`gitlab`这个东西初步了解了一下主要是面向企业和学校的，它可以构建`github`类似的仓库;

----

<center>2023.2.21来更新一下</center>

OpenSSL SSL_read: Connection was reset, errno 10054报错无法push[解决办法](https://blog.csdn.net/sinat_32017511/article/details/115762643)，有人说是因为dns被污染的问题，我们只需要用`git init`之后再`git push`就可以了。

# git的使用
---
## git安装后的初始化
    `git config --global user.name "youname"`
    `git config --global user.email "youEmail"`
---
## git 创建一个版本库
```shell
#在需要变成版本库的目录下
git init
```
---
## git '时光穿梭机'
**小结**
>* 要随时掌握工作区的状态 `git status`
>* 如果 `git status` 告诉你有文件被修改过， 可以使用 `git dff`查看被修改的内容
---
### 版本回退

**小结**
>* `head`指向的版本就是当前版本,可以使用命令`git reset --hard commit_id`穿梭版本
>* 穿梭前，用`git log`可以查看提交历史，以便确定要回退到哪个版本。
>* 要重返未来，用`git reflog`查看命令历史，以便确定要回到未来的哪个版本。
>* `git log [--pretty=oneline]`显示提交日志
>* `git reset --hard ****`后面是版本号 不需要打全
```

```
---

### 工作区和暂存区
**小结**

>* 工作区就是电脑能看到的目录,作为版本的目录
>* 工作区有一个隐藏目录.git，这个不算工作区，而是Git的版本库。
>* 暂存区就是Git的版本库里存了很多东西，其中最重要的就是称为stage（或者叫index）的暂存区，还有Git为我们自动创建的第一个分支master，以及指向master的一个指针叫HEAD。

![](https://static.liaoxuefeng.com/files/attachments/919020074026336/0)!
![](https://www.liaoxuefeng.com/files/attachments/919020100829536/0)!

---

### 管理修改
>* 提交后，用`git diff HEAD -- readme.txt`命令可以查看工作区和版本库里面最新版本的区别：
>* `git add filename` 将文件添加到暂存区
>* `git commit -m "message"` 暂存区内容提交版本 
---


#### 一、下载地址
https://git-scm.com/download/win

#### 二、配置命令
`git config --global user.name "itheima"`
`git config --global user.email "itheima@itcast.cn"`

#### 三、查看配置信息
1、记事本查看：C:/Users/用户名文件夹/`.gitconfig`
2、命令行查看：
① 查看所有的全局配置项  `git config --list --global`  

② 查看指定的全局配置项 `git config user.email`

#### 四、获取帮助信息

1、打开`git config`命令的帮助手册: `git help config`

2、获取`git config`命令的快速参考: `git config -h`

#### 五、获取 `Git` 仓库的两种方式

 1、将尚未进行版本控制的本地目录转换为 Git 仓库: `git init`

①查看文件状态： `git status`     `git status -s`

②跟踪新文件:  `git add 文件名`

③提交更新: `git commit  -m "信息描述"`

④对已提交的文件进行修改

>  工作区中文件的 4 种状态：
>
> ①未跟踪（Untracked）
>
> ②未修改（Unmodified）
>
> ③已修改（Modified）
>
> ④已暂存（Staged）

⑤暂存已修改的文件：`git add 文件名`

⑥提交已暂存的文件： `git commit -m "提交消息"` 

⑦撤销对文件的修改：`git checkout --文件名`

⑧向暂存区中一次性添加多个文件：`git add .`

⑨取消暂存的文件：`git reset HEAD  要移除的文件名称`

⑩跳过使用暂存区域：`git commit -a -m "描述信息"`

⑾移除文件：

从`git`仓库和工作区中同时移除：`git rm -f 移除的文件名`       

只从`git`仓库中移除：`git rm --cached "移除的文件名"`

⑿忽略文件：创建一个名为 `.gitignore` 的配置文件

⒀查看提交历史：`git log(--pretty oneline)`；在旧版本中使用 `git reflog --pretty=oneline`命令，查看命令操作的历史

⒀版本回退：`git reset --hard <CommitID>`

2、从其它服务器克隆一个已存在的 `Git` 仓库


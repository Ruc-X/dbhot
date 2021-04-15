## git
### 三大区域
- 工作区 红色
    - 已管
    - 新增
    - git add 工作区 => 暂存区
- 暂存区 绿色  
    - git commit 暂存区 => 版本库
- 版本库
### 小命令
- 管理目录下的文件状态
``` git
git status 
注：新增的文件和修改过后的文件都是红色
```
- 管理指定文件(红变绿)
``` git
git add 文件名
git add .
```
- 个人信息配置： 用户名、邮箱 **[一次即可]**
``` git
git config --global user.email "you@example.com"
git config --global user.name "Your Name"
```
- 生成版本
``` git
git commit -m '描述'
```
- 查看版本记录
``` git
git log
``` 
- 拓展新功能
``` git
git add 
git commit -m '新功能'
```
- 回滚至之前版本
```git 
git log
git reset --hard 版本号
```
- 回滚至之后的版本
``` git
git reflog
git reset --hard <版本号>  //回滚
```
- 红变白
``` git
git check out -- 文件名
```
- 绿变红
``` git
git reset HEAD 文件名
```

### 分支
- 保留改变的代码，未改变的用指针指向原来的版本，分支在主干基础上分别开发
- 环境隔离
- 命令总结
    - 查看分支
    ``` git
    git branch
    ```
    - 创建分支
    ``` git
    git branch 分支名称
    ```
    - 切换分支
    ``` git
    git checkout 分支名称
    ```
    - 分支合并 ：可能产生冲突
    ``` git
    git merge 要合并的分支
    注意：切换分支到主分支再合并需要被合并的分支
    ```
    - 删除分支
    ``` git
    git brach -d 分支名称
    ```
### github
``` git
git init
git add README.md
git commit -m 'first commit'
git remote add origin https://github.com/Ruc-X/dbhot.git
```
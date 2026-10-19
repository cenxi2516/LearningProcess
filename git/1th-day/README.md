# git核心概念和命令

## 配置

### 配置命令

```bash
git config -l # 查看当前生效的所有配置  git config list简写
git config 键 # 查看当前生效的某个配置的值
git config --范围 键 "值" # 更新配置
```

### 配置范围

- `worktree`：仅对当前工作树生效
- `local`：【常见】【默认】仅对当前仓库有效
- `global`：【常见】对当前用户的所有仓库有效
- `system`：对所有用户有效

优先级：`worktree` > `local` > `global` > `system`

### 常见配置

- `name.user`：【必配】配置用户名。后续提交会使用该用户名。
- `name.email`: 【必配】配置邮箱。后续提交会使用该邮箱。
- `core.editor`: 配置默认文本编辑器。
- `core.ignorecase`: 配置是否忽略文件名的大小写。默认是`true`，即忽略大小写。
- `init.defaltbranch`: 配置初始化后默认的分支名。

```bash
git config --global user.name 'Your's name'
git config --global user.email 'Your's email'
git config --global core.editor 'code --wait'
git config --global core.ignorecase false
git config --global init.defaultbranch 'main'
```

## 初始化

要对一个目录使用git进行版本管理，必须先将该目录设置为git仓库。
使用 `git init` 命令初始化一个新的git仓库。
该命令会在当前目录下创建一个`.git`目录，该目录就是git仓库，里面记录了仓库的所有信息。该目录不可删除，一旦删除，该仓库就不存在了。

## .gitignore文件

仓库中某些文件是「个人专属」，不会在团队共享，可以使用`.gitignore`文件将不需要的文件排除。

### git-merge

[![GitHub release](https://img.shields.io/github/release/monlor/git-merge.svg)](https://github.com/monlor/git-merge/releases)

### 安装教程

#### 【推荐】brew安装（[brew](https://brew.sh/index_zh-cn)支持WSL/Linux/Mac）

```
➜ brew tap monlor/taps
➜ brew install git-merge
➜ brew upgrade git-merge # 脚本更新命令
```

#### 手动安装（假设安装到~/Document）

* 到[`latest release`](https://github.com/monlor/hcf-pack/releases/latest)下载`Source code`

  ![](https://file.monlor.com/img/20200109111107.png)

* 解压到`~/Document`

* 添加`~/Document/git-merge`到环境变量PATH


### 开始使用

* 在`git`项目目录中执行`gitmerge`，提示生成一个项目环境变量文件
* 程序会在家目录下的`.project`目录中生成一个文件夹，文件夹命名方式为：**项目组名称_项目名称**
* 修改`gitmerge.env`中的配置，完成之后继续在`git`项目目录中执行`gitmerge`

#### 使用命令说明

```
➜ gitmerge [dev/uat/prod 或 分支名]
```

* 执行此命令程序会以当前分支作为来源分支，参数一为目标分支，提一个合并请求
* `dev/uat/prod`在环境变量中配置后，会转换成相应的分支名。比如执行命令`gitmerge dev`，`dev`分支名配置的是`dev-latest`，那么会提合并请求到`dev-latest`

#### 获取`PRIVATE_TOKEN`

![](https://file.monlor.com/img/20200109110806.png)

![](https://file.monlor.com/img/20200109110834.png)

![](https://file.monlor.com/img/20200109110855.png)
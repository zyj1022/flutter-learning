# 搭建Flutter开发环境

由于Flutter会同时构建Android和IOS两个平台的发布包，所以Flutter同时依赖Android SDK和iOS SDK，在安装Flutter时也需要安装响应平台的构建工具和SDK。

## 使用镜像

由于在国内访问Flutter有时可能会受到限制，Flutter官方为中国开发者搭建了临时镜像，大家可以将如下环境变量加入到用户环境变量中：

***Mac 用户环境变量***

打开如下路径文件，
```
~/.bash_profile
```
添加

```
export PUB_HOSTED_URL=https://pub.flutter-io.cn
export FLUTTER_STORAGE_BASE_URL=https://storage.flutter-io.cn
```

## 在masOS下可以同时进行Android和iOS设备的测试。

### 系统要求

要安装并运行Flutter，您的开发环境必须满足以下最低要求:

- 操作系统: macOS (64-bit)
- 磁盘空间: 700 MB (不包括Xcode或Android Studio的磁盘空间）.
- 工具: Flutter 依赖下面这些命令行工具.
`bash`、`mkdir`、`rm`、`git`、`curl`、`unzip`、`which`


## 获取Flutter SDK

1、去flutter官网下载其最新可用的安装包，官网地址：https://flutter.io/sdk-archive/#macos

### 更新环境变量

将Flutter添加到PATH中，可以在任何终端会话中运行flutter命令。

对于所有终端会话永久修改此变量的步骤是和特定计算机系统相关的。通常，您会在打开新窗口时将设置环境变量的命令添加到执行的文件中。例如

1、确定您Flutter SDK的目录记为`“FLUTTER_INSTALL_PATH”`，您将在步骤3中用到。

2、打开(或创建) `$HOME/.bash_profile`。文件路径和文件名可能在你的电脑上不同.

3、添加以下路径:

```
export PATH=[FLUTTER_INSTALL_PATH]/flutter/bin:$PATH
```
例如笔者Flutter 安装目录是“~/code/flutter_dir”，那么代码为：

```
export PATH=~/code/flutter_dir/flutter/bin:$PATH
```
4、运行 `source $HOME/.bash_profile `刷新当前终端窗口。

注意: 如果你使用终端是zsh，终端启动时 `~/.bash_profile` 将不会被加载，解决办法就是修改 `～/.zshrc` ，在其中添加：`source ～/.bash_profile`

5、验证“flutter/bin”是否已在PATH中：

```
echo $PATH
```

## 安装 Xcode

安装Xcode 9.0或更新版本.
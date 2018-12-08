# VS Code的配置与使用

VS Code是一个轻量级编辑器，支持Flutter运行和调试。

## 安装flutter插件

- 启动 VS Code。
- 调用 View>Command Palette…。
- 输入 ‘install’, 然后选择 Extensions: Install Extension action。
- 在搜索框输入 flutter ，在搜索结果列表中选择 ‘Flutter’, 然后点击 Install。
- 选择 ‘OK’ 重新启动 VS Code。

- 验证配置
    - 调用 View>Command Palette…
    - 输入 ‘doctor’, 然后选择 ‘Flutter: Run Flutter Doctor’ action。
    - 查看“OUTPUT”窗口中的输出是否有问题

## 创建Flutter应用

- 启动 VS Code
- 调用 **View>Command Palette**…
- 输入 ‘flutter’, 然后选择 ‘Flutter: New Project’ action
- 输入 Project 名称 (如myapp), 然后按回车键
- 指定放置项目的位置，然后按蓝色的确定按钮
- 等待项目创建继续，并显示main.dart文件

## 体验热重载

- 打开lib/main.dart文件。
- 将字符串 `'You have pushed the button this many times:'` 更改为 `'You have clicked the button this many times:'`。
- 不要按“停止”按钮; 让您的应用继续运行。
- 要查看您的更改，请调用 `Save (cmd-s / ctrl-s)`, 或者点击 热重载按钮 (绿色圆形箭头按钮)。
- 你会立即在运行的应用程序中看到更新的字符串。
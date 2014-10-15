Markdown PPT
============

Markdown PPT 是一款将 Markdown 文件转换成简单 PPT 文件显示的小工具。

## 语法

遵循 Markdown 语法，使用水平线 `hr` 将 Markdown 内容分割成 PPT 页。

**Markdown**

```
************

OR

* * *
```

**示例**

https://github.com/aiyanbo/md-ppt/blob/master/sample/sample.md

## 开始使用

1. 按照标准格式书写 markdown 文件
2. 打开播放器程序 http://aiyanbo.github.io/md-ppt/player.html
3. 将 markdown 文件拖入 "Drop markdown file" 框中

### Air-Play 功能使用

1. 启动 Air-Play 服务 (操作方式参考 https://github.com/aiyanbo/md-ppt#多屏互动)
2. 在程序界面上的 Air Play 文本看输入服务地址
3. 输入完成后按 回车 键连接
4. 连接成功之后，点击 Pin Code 按钮(6位数字)
5. 将分享连接复制给其他子屏幕
6. 移动设备可以使用 微信 微博 QQ 等工具扫墓二维码

## 操作

### PC 端

- 向左剪头 --> 上一页
- 向右剪头 --> 下一页

### 移动设备

- 向左滑动 --> 下一页
- 向右滑动 --> 上一页

## 多屏互动

Markdown PPT 现已实现多屏互动，但暂时需要安装本地服务端。使用方式为：

- 安装并启动 `air-play` 服务端

```
cd air-play
npm install
node server.js
```

- 打开程序 http://aiyanbo.github.io/md-ppt/player.html
- 在 Air Play 文本输入框中输入服务器地址。例如：`ws://localhost:8001`
- 连接成功后，点击 Pin Code 按钮(有6位数字)。
- 分享连接给其他屏幕，也可以使用移动端扫描二维码。

> **Notes**
> 主控制器(一般是您的移动设备)请将 Read only 选项关闭。

## 使用的组件

- jQuery
- jQuery mobile
- ZeroClipboard
- CommonMark http://commonmark.org/
- Bootstrap http://getbootstrap.com/

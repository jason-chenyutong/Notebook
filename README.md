# Notebook - 简易文本编辑器

一个基于 Python Tkinter 构建的轻量级桌面文本编辑器，提供基础的文本编辑功能和中文菜单界面。

## 功能特性

- **新建文件** - 创建新的文本文件并选择保存路径（Ctrl+N）
- **打开文件** - 打开已有的文本文件进行编辑（Ctrl+O）
- **保存文件** - 将当前编辑内容保存到文件（Ctrl+S）
- **退出程序** - 关闭编辑器（Ctrl+Q）
- **自定义背景色** - 右键菜单选择编辑区背景颜色

## 环境要求

- Python 3.x
- Tkinter（Python 标准库，通常随 Python 一起安装）

> Linux 系统可能需要单独安装：`sudo apt install python3-tk`

## 运行方式

```bash
python gui.py
```

## 打包为可执行文件

项目提供了 PyInstaller 打包配置，可将程序打包为独立的 Windows 可执行文件：

```bash
pip install pyinstaller
pyinstaller gui.spec
```

打包完成后，可执行文件将生成在 `dist/` 目录下。

## 项目结构

```
notebook/
├── gui.py          # 应用程序主代码
├── gui.spec        # PyInstaller 打包配置
├── build/          # PyInstaller 构建产物
└── README.md
```

## 技术栈

| 组件     | 技术         |
| -------- | ------------ |
| 编程语言 | Python       |
| GUI 框架 | Tkinter      |
| 打包工具 | PyInstaller  |

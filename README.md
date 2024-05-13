# termdebug

`Termdebug` 是一个基于vim终端模拟器(vim 8.1+ 或 neovim 0.3.6+)的调试插件。

当前, termdbg支持
- pdb (pdb3) 
- ipdb (ipdb3)
- lldb
- dlv (go Delve)

如果你需要gdb支持, 请尝试termdebug (`:h termdebug`)

当前, termdbg支持以下功能:

- 当调试时, 将光标定位到当前运行行
- 简单的在buffer中切换断点

## 安装

> 需要vim 8.1+ (+terminal) 和 neovim 0.3.6+.

### vim-plug

```viml
Plug 'IammyselfYBX/termdbg'
```

### 手动安装

- Extract the files and put them in your .vim directory
  (usually `~/.vim`).

## 使用

使用: `Termdbg {debugger} {file} [args]`

例子: `Termdbg ipdb3 a.py`

## Commands

- `:TNext` 跳过当前行
- `:TStep` 进入当前行
- `:TFinish` 返回当前函数
- `:TContinue` 运行到下一个断点
- `:TLocateCursor` 将光标定位到当前运行行
- `:TToggleBreak` 在当前行切换断点
- `:TSendCommand` 发送命令到调试器





# termdbg

Termdbg is a terminal debugger plugin for vim 8.1+ and neovim 0.3.6+.  
Currently, termdbg supports
- pdb (pdb3)
- ipdb (ipdb3)
- lldb
- dlv (go Delve)

If you need gdb support, try termdebug (`:h termdebug`)

Currently, termdbg just only do these things:
- locate cursor to current running line when debugger
- simply toggle breakpoints in buffer

## Install

> Need vim 8.1+ (+terminal) and neovim 0.3.6+.

### vim-plug

```viml
Plug 'IammyselfYBX/termdbg'
```

### 手动安装

- Extract the files and put them in your .vim directory
  (usually `~/.vim`).

## Usage

Usage: `Termdbg {debugger} {file} [args]`

Example: `Termdbg ipdb3 a.py`

## Commands

- `:TNext` Step over
- `:TStep` Step in
- `:TFinish` Return from current function
- `:TContinue` Continue
- `:TLocateCursor` Locate cursor to running line
- `:TToggleBreak` Toggle breakpoint in current line
- `:TSendCommand` Send command to debugger


## Options
None.


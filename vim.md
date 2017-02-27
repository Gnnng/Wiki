
Vim
======


参数设置
----

> 以下命令均可加 `no` 前缀来禁用

- `set foldenable`: 启用缩进
- `set hlsearch`: 启用搜索高亮
- `set number`: 启用行号
- `set colorcolumn=80`: 设置 line ruler 为 80


命令
----

- `:%s/foo/bar/gc`
    - `%`:指定搜索范围为全文
    - `g`: 全局
    - `c`: 需要确认
- `:w !sudo tee %` 
    - `%`:当前文件名


YouCompleteMe
------

更新之后需要重新编译

```
cd ~/.vim/bundle/YouCompleteMe
./install.py --clang-completer --gocode-completer  --tern-completer
```

参数分别为:

- `clang-completer`: C-family language support
- `gocode-complter`: Golang support
- `tern-complter`: Nodejs support


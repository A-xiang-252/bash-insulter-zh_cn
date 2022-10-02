# bash-insulter-中文版
当输入错误命令时，随机侮辱用户

原项目地址[bash-insulter](https://github.com/hkbakke/bash-insulter)

对原项目增加了中文翻译，未增添或减少嘲讽内容

根据你的需要更改嘲讽内容

例如：

```bash
noob@bender:~ $ sl

  Y u no speak computer???

-bash: sl: command not found
noob@bender:~ $ gti status

  This is why nobody likes you.

-bash: gti: command not found
noob@bender:~ $ sp aux

  Go outside.

-bash: sp: command not found
```

# 兼容
* Bash v4 或更新的版本
* Zsh

# 安装和配置

1.克隆这个项目

    # 使用git
    git clone https://github.com/A-xiang-252/bash-insulter-zh_cn.git bash-insulter
    sudo cp bash-insulter/src/bash.command-not-found /etc/

    # 使用wget
    sudo wget -O /etc/bash.command-not-found https://github.com/A-xiang-252/bash-insulter-zh_cn/blob/master/src/bash.command-not-found

2.配置

使用编辑器，如 `vim` ，编辑你的 ~/.bashrc 或者 /etc/bash.bashrc 文件

添加以下内容

```
if [ -f /etc/bash.command-not-found ]; then
    . /etc/bash.command-not-found
fi
```
重新登录并输入一些无效的命令来查看效果。


注意: 如果你是用的是 `zsh` ,你必须将脚本添加到 `.zshrc`

【剩余内容请查看原项目(主要是因为看不懂了😂)】

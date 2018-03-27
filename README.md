# item2
mac终端快速启动Sublime/WebStrom/VS Code/Atom等编辑器

考虑你是ZSH

输入命令j, 会提示 zsh: command not found: j

是因为没有安装autojump插件，在~/.zshrc文件中找到plugins=()改为plugins=(autojump)

然后使用别名的方式为webstorm设置一下命令，如：alias ws="wstorm”

全部配置好发现仍然无法用ws命令打开，这个时候需要配置webstorm，在”Tools” -> “Create Command Line Launcher…” 设置命令，这样就可以直接打开了，大功告成！

三步必须全部设置，才能正常打开。

```
alias atom='/Applications/Atom.app/Contents/MacOS/Atom'
// sublime3
alias subl='/Applications/Sublime\ Text.app/Contents/SharedSupport/bin/subl'
// sublime2
alias subl='/Applications/Sublime\ Text\ 2.app/Contents/SharedSupport/bin/subl' 
alias code='/Applications/Visual\ Studio\ Code.app/Contents/Resources/app/bin/code'
//webstorm 在命令行中用ws命令打开webstorm
alias ws="/usr/local/bin/webstorm"
```

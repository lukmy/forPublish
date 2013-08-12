安装流程:

- 更新xcode
	- 安装cmd-line tools
- (optional) [iterm2](http://www.iterm2.com/)
- 安装[homebrew](https://github.com/mxcl/homebrew)

检查homebrew是否有问题, 终端下运行

> brew doctor

如果没问题, 运行

> brew update

使用homebrew安装git

> brew install git

安装oh my zsh

> curl -L https://github.com/robbyrussell/oh-my-zsh/raw/master/tools/install.sh | sh

设置默认shell为zsh

> sudo chsh -s /bin/zsh *username*

#### zsh的优点

zsh有着更为强大的命令行补全方式, 能够提供更为详尽的命令选项, 在使用的时候不必要去查阅文档.

另外, 经过适当的配置, zsh可以有一些很实用的功能. 如: 打路径不需要区分大小写(cd jenkins补全cd Jenkins), 只需要打一部分关键词就能够补全出命令(用art补全start). 

#### zsh的配置

在OSX上有一个已经被优化的很神的zsh配置, 叫oh my zsh, 基本上是一键配置了. 大概装好之后就能用. 可以有一些自定义的优化, 没事的时候玩玩挺有趣.


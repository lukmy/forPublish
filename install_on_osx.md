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

oh my zsh配置好了之后, 重新进入zsh, 可以看到zsh有一些很神奇的功能. 

- 数字键可以对应之前进入的目录, 如之前依次进入 `/usr` `~/Documents` `/etc` 目录, 当前在 `~/Downloads` 则对应关系:

目录 		| 数字
-----------	| ----
~/downloads | 
/etc		| 1
~/Documents	| 2
/usr		| 3

但一般不这么写, 用得比较多的一个方法是一直按某个数字轮转.

- 不需要输入cd, 直接输入路径就能切换到相应目录

`cd /usr/local/bin` -> `/usr/local/bin`

- 结合autojump, 可以快速的跳转

autojump是一个快速跳转工具, 安装完之后, 会记录从autojump安装之后所切换过的所有路径. 并判断关键词快速切换.

`autojump in` -> `cd /usr/local/bin`

autojump会找到切换过的路径中符合输入关键词的切换次数最多的那条直接切换到那个地方. 

oh my zsh将autojump进行了简化, 可以使用`j keyword`来跳转.

可以使用 `brew install autojump` 来安装autojump

> 要使用`j`, 需要在~/.zshrc中把plugins那行加入autojump

### bash的加强

> brew install bash-completion

安装完了之后会有一段话, 那段话会要求将一段文字加入~/.bashrc中, 需要到时候加上, 不然bash-completion无法使用

### git的图形化用具

[Source Tree](http://www.sourcetreeapp.com/)

比gitk做的更好的一个图形化git工具, 和github也有集成, 甚至还有git flow的支持. 同时也支持mecurial.

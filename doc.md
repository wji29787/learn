# 开发环境搭建

<a name="SbLWg"></a>

## 软件安装

mac 软件推荐系列：[https://github.com/qianguyihao/Mac/blob/master/01-Mac%E8%BD%AF%E4%BB%B6%E6%B1%87%E6%80%BB.md](https://github.com/qianguyihao/Mac/blob/master/01-Mac%E8%BD%AF%E4%BB%B6%E6%B1%87%E6%80%BB.md)<br />切勿安装盗版软件

- sketch -
- charles -
- Xmind8 -
- [chrome](https://www.google.com/chrome/?brand=CHBD&gclid=EAIaIQobChMI78W-j6iJ4wIVFz5gCh3HyAt3EAAYASAAEgLiNfD_BwE&gclsrc=aw.ds) - 自行下载安装

- [iTerm2](https://www.iterm2.com/) - mac 系统中不可多得的命令行工具之一.
- [brew](https://brew.sh/index_zh-cn) - Mac OS 平台下的软件包管理工具，拥有安装、卸载、更新、查看、搜索等很多实用的功能。简单的一条指令，就可以实现包管理，而不用你关心各种依赖和文件路径的情况，十分方便快捷
- [nodejs](https://nodejs.org/en/) - brew install nodejs
- [Sourcetree](https://www.sourcetreeapp.com/) -  是 Windows 和 Mac OS X 下免费的 Git 和 Hg 客户端，拥有可视化界面，容易上手操作
- [Visual Studio Code](https://code.visualstudio.com/) - 前段必备编辑器
- [git](https://git-scm.com/) - brew install git
- [oh-my-zsh](https://github.com/robbyrussell/oh-my-zsh)
- xcode - 在 App Store 里面下载安装。如果不能安装，应该是要先升级电脑系统
- [Spectacle](https://www.spectacleapp.com/) - 分屏软件，方面你管理桌面窗口

<a name="ZqTDm"></a>

## 软件配置

<a name="9oruT"></a>

### vim 配置

set nocompatible                " 关闭 vi 兼容模式<br />
syntax on                            " 自动语法高亮<br />
set number                          " 显示行号<br />
set cursorline                      " 突出显示当前行<br />
set ruler                              " 打开状态栏标尺<br />
set shiftwidth=4                  " 设定 << 和 >> 命令移动时的宽度为 4<br />
set softtabstop=4              " 使得按退格键时可以一次删掉 4 个空格<br />
set tabstop=4                      " 设定 tab 长度为 4<br />
set cindent                           "语言的自动缩进方式<br />
autocmd InsertLeave _ se nocul<br />
autocmd InsertEnter _ se cul  " 用浅色高亮当前行<br />
set autoindent                        " 自动对齐<br />
set confirm                             " 在处理未保存或只读文件的时候，弹出确认<br />
set incsearch                          " 输入搜索内容时就显示搜索结果<br />
set hlsearch                            " 搜索时高亮显示被找到的文本<br />
set magic                                " 设置魔术<br />
set hidden                               " 允许在有未保存的修改时切换缓冲区，此时的修改由 vim 负责保存<br />
set smartindent                       " 开启新行时使用智能自动缩进

<a name="VcK54"></a>

### vscode 配置

open vscode in iterm2<br />
Try this one<br />
Open Visual Studio Code and press Command + Shift + P then type `Shell` in command palette now you are able to find this option like `Shell Command : Install code in PATH` from suggested list in command palette. Select that options.<br />
<br />
下载 Settings Sync 插件，配置好，可上传下载 vscode 所有配置以及安装的所有插件<br />
1、在 github 上生生 token<br />
2、拷贝之前的 sync.gist

<a name="nQtu5"></a>

#### 推荐安装插件：

- **Auto Close Tag** - Automatically add HTML/XML close tag
- **Auto Rename Tag** - Auto rename paired HTML/XML tag
- **Beautify** - Beautify code in place for VS Code
- **Code Runner** - Run C, C++, Java, JS, PHP, Python, Perl, Ruby, Go, Lua, Groovy, PowerShell, CMD, BASH, F#, C#, VBScript, TypeScript, CoffeeScript, Scala, Swift, Julia, Crystal, OCaml, R, AppleScript, Elixir, VB.NET, Clojure, Haxe, Obj-C, Rust, Racket, AutoHotkey, AutoIt, Kotlin, Dart, Pascal, Haskell, Nim, D, Lisp
- **EditorConfig for VS Code** - EditorConfig Support for Visual Studio Code
- **ES7 React/Redux/GraphQL/React-Native snippets** - Simple extensions for React, Redux and Graphql in JS/TS with ES7 syntax
- **ESLint** - Integrates ESLint JavaScript into VS Code.
- **Git History** - View git log, file history, compare branches or commits
- **GitLens** — Git supercharged - Supercharge the Git capabilities built into Visual Studio Code — Visualize code authorship at a glance via Git blame annotations and code lens, seamlessly navigate and explore Git repositories, gain valuable insights via powerful comparison commands, and so much more
- **markdownlint** - Markdown linting and style checking for Visual Studio CodeMaterial Theme - The most epic theme now for Visual Studio Code
- **One Dark Pro** - Atom's iconic One Dark theme for Visual Studio Code
- **SVG Viewer** - SVG Viewer for Visual Studio Code.
- **Trailing Spaces** - Highlight trailing spaces and delete them in a flash!
- **View In Browser **- view a html file in system's default browser
- **Settings Sync** - Synchronize Settings, Snippets, Themes, File Icons, Launch, Keybindings, Workspaces and Extensions Across Multiple Machines Using GitHub Gist.
- **Toggle Quotes**  britesnow.vscode-toggle-quotes 
  Toggle cycle " -> ' -> `

<a name="Qmgtm"></a>

### [Oh My Zsh](https://github.com/robbyrussell/oh-my-zsh)

安装 ZSH<br />`sh -c "$(curl -fsSL https://raw.githubusercontent.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"`
<a name="jmzgr"></a>

#### 设置主题

- **安装完毕后，我们就可以使用了，先来简单配置一下，Oh My Zsh 提供了很多主题风格，我们可以根据自己的喜好，设置主题风格**
- 终端输入命令  **open ~/.zshrc**。
- 找到  **ZSH_THEME ，ZSH_THEME="robbyrussell" ，robbyrussell** ，是默认的主题，修改  **ZSH_THEME="样式名称"**
- 保存这个文件文件，重新打开终端。
  <a name="W5gzv"></a>

#### 随机主题

- 设置 ZSH_THEME="random", 每次打开终端主题是随机的，如果遇到一个你喜欢的，你再写死配置
- source ~/.zhsrc 随时随地换主题，不喜欢就运行一下换个新鲜的

<a name="b75wl"></a>

#### 查看已安装主题名称

`ls ~/.oh-my-zsh/themes`

<a name="j5EZm"></a>

#### git 插件

打开 ~/.zshrc 找到 plugins=(git) 这一行，添加上 git 就行<br />[git 命令简写](https://github.com/robbyrussell/oh-my-zsh/tree/master/plugins/git/)

<a name="U8Lnf"></a>

### Spectacle

<br />在  **设置>安全性与隐私>辅助功能**  勾选 Spectacle.app<br />在  **设置>用户与群组>登录项**  勾选 Spectacle，启用开机启动

窗口管理快捷键如下，可自行修改配置。
<a name="8Pb4p"></a>

## ![image.png]()

<a name="tPoax"></a>

<a name="7srbD"></a>

### sourcetree 安装

1、打开 sourcetree<br />2、关闭 sourcetree<br />3、命令终端输入`defaults write com.torusknot.SourceTreeNotMAS completedWelcomeWizardVersion 3`<br />4、打开 sourcetree 即可跳过登录<br />

# 几款不错的在线流程图绘制工具

- draw: [https://www.draw.io/](https://www.draw.io/)，简洁，功能强大，免费
- gliffy: [https://www.gliffy.com](https://www.gliffy.com)，简洁，功能强大，免费
- processon: [https://processon.com](https://processon.com)，简洁，功能强大，半免费
- whimisical: [https://whimsical.com/flowcharts/](https://whimsical.com/flowcharts/)，好看，功能简单，免费
- asciiflow: [http://asciiflow.com](http://asciiflow.com)，简洁，全字符，免费

asciiflow 是全字符的，适合在代码、命令行等环境中使用，draw 和 gliffy 的功能是比较相似的，后者在体验上稍好，processon 提供了丰富的母版，并且把社区做起来了，免费空间不多，但是体验挺好，whimisical 最近才知道，比较华丽，但是功能稍微简洁一点

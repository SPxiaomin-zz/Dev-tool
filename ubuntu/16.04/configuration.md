### 系统配置（16.04）

- Terminal 主题设置

    - profiles -> profile preferences -> Colors -> Built-in schemes: Solarized light、Solarized、Use transparency from system theme
    
- 更新（可能需要多输入几次）

    - sudo apt update
    - sudo apt upgrade

- GIT

    - 安装 git
    
        - sudo apt install git

    - 生成 ssh key，并添加到 github 上去

        - ssh-keygen -t rsa -C "3013366498@qq.com"

    - git 设置

        - git config --global user.email "3013366498@qq.com"
        - git config --global user.name "gujunmin"
        - git config --global push.default matching
        - git config --global alias.st status
        - git config --global alias.co checkout
        - git config --global alias.ci commit
        - git config --global alias.br branch
        - git config --global alias.unstage 'reset HEAD'
        - git config --global alias.last 'log -1'
        - git config --global alias.lg "log --color --graph --pretty=format:'%Cred%h%Creset -%C(yellow)%d%Creset %s %Cgreen(%cr) %C(bold blue)<%an>%Creset' --abbrev-commit"

- zsh

    - 安装 zsh

        - sudo apt install zsh
        - chsh -s $(which zsh)

            - 注意: 电脑重启才可以生效

    - oh-my-zsh

        - sh -c "$(curl -fsSL https://raw.githubusercontent.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"

    - 自定义 shell script 设置

        - 修改 ~/.zshrc

            - PATH
            - 执行权限 chmod a+x filename
            - 设置 alias 使得 script 在当前的 shell 环境中执行

    - 修改 ~/.zshrc 文件

- vim 安装

    - sudo apt-get install vim

    - 设置 ~/.vimrc

    - 安装和设置 Vundle

        - <https://github.com/VundleVim/Vundle.vim>

- 软件安装工具下载

    - sudo apt install gdebi

- Chrome 安装

- 搜狗输入法安装

- 翻墙

    - 安装 pip

        - sudo apt install pip

    - 使用 pip 安装 shadowsocks

        - pip install shadowsocks

    - 开启代理

        - sslocal -s 'server' -p port -k 'password' -m 'rc4-md5'

    - 安装 google chrome 翻墙插件并设置 protocol: sock5，server: 127.0.0.1，port: 1080 

- Atom 安装

    - sudo add-apt-repository ppa:webupd8team/atom

    - sudo apt-get update

    - sudo apt-get install atom

- VirtualBox

    - 安装

        - sudo apt install virtualbox

    - 设置全屏模式

        - Devices -> Insert Guest Additions CD Image

    - 设置共享文件夹

        - <http://jingyan.baidu.com/article/647f0115ab16f17f2048a861.html>

    - 设置共享黏贴板

        - Devices -> Shared Clipboard > Bidirectional

    - 安装 qq

    - 安装百度云管家

    - 安装 ps

        - 破解 ps

        - ps 设置

            - 移动工具设置为选择图层

            - 视图

                - 显示 -> 智能参考线

                - 标尺

            - 窗口

                - 关闭

                    - 库
                    - 颜色

                - 打开

                    - 图层

                    - 信息

                        - 面板选项

                            - 第一颜色信息

                                - RGB 颜色

                            - 第二颜色信息

                                - RGB 颜色

                            - 鼠标坐标

                                - 像素

                            - 状态信息

                                - 文档尺寸

                    - 字符

            - 编辑

                - 首选项 -> 单位与标尺

                    - 单位

                        - 像素

            - 新建工作区

                - 窗口

                    - 工作区 -> 新建工作区（选项全部勾上）

    - 安装 as

- wps 安装

    - sudo apt-get install wps-office

- tree 安装

    - sudo apt install tree

- node 开发环境安装设置

    - 安装 nvm

        - cd ~/gitProject

        - git clone https://github.com/creationix/nvm.git

        - 在 ~/.zshrc 文件中添加
        
            - export NVM_NODEJS_ORG_MIRROR=https://npm.taobao.org/dist

            - source ~/gitProject/nvm/nvm.sh

    - 安装 node

        - nvm ls-remote 选择最新版本的 node，然后 nvm install <version>

    - 修改 npm 的源

        - 创建 ~/.npmrc 文件

            - 添加 registry=https://registry.npm.taobao.org

    - 安装 cnpm

        - npm install -g cnpm --registry=https://registry.npm.taobao.org

- 安装 eslint

    - cnpm i -g eslint

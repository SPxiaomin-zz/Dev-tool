### 系统配置（16.04）

- Terminal 主题设置

	- profiles -> profile preferences -> Colors -> Built-in schemes: Solarized light、Use transparency from system theme

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

- vim 安装

	- sudo apt-get install vim

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

- wps 安装

	- sudo apt-get install wps-office


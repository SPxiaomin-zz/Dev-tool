### 系统配置（16.04）

- 软件安装工具下载

	- sudo apt install gdebi

- 翻墙

	- 安装 pip

		- sudo apt install pip

	- 使用 pip 安装 shadowsocks

		- pip install shadowsocks

	- 开启代理

		- sslocal -s 'server' -p port -k 'password' -m 'rc4-md5'

	- 安装 google chrome 翻墙插件并设置 protocol: sock5，server: 127.0.0.1，port: 1080 

- GIT

	- 安装 git
	
		- sudo apt install git

	- 生成 ssh key，并添加到 github 上去

		- ssh-keygen -t rsa -C "3013366498@qq.com"

#### 第三方软件安装

- Atom 安装

	- sudo add-apt-repository ppa:webupd8team/atom

	- sudo apt-get update

	- sudo apt-get install atom

- Chrome 安装

- 搜狗输入法安装

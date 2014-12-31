天马伴侣
=============

如果你知道什么是[天马服务器](http://nqdeng.github.io/tianma/)，并且对Apache为Windows系统提供的托盘程序感到特别羡慕的话，可以试试看天马伴侣。

### 系统要求

目前只支持Windows系统。Windows XP用户需要先安装`.NET Framework 2.0`，Windows Vista和Windows 7用户不需要做啥，Windows 8用户请在运行天马伴侣时根据系统提示安装`.NET Framework 3.5`。


### 如何安装

>	[http://tianmajs.github.io/tianma.daemon/tianmad-latest.zip](http://tianmajs.github.io/tianma.daemon/tianmad-latest.zip)

从以上位置下载压缩包后，将里边的`tianmad.exe`解压到包含天马配置文件的工作目录里。

	+ www/
		+ certificates/
		+ htdocs/
		config.js
		tianmad.exe    <= 放在这里

### 如何使用

双击之后，天马伴侣就会使用默认配置文件（config.js）启动服务，并在系统托盘里创建一个小图标。在小图标上右键单击后会出现以下菜单：

	+----------+
	| Switch > |   <= 切换当前服务使用的配置文件并重启服务
	| -------- |
	| Start    |   <= 启动当前服务
	| Stop     |   <= 停止当前服务
	| Restart  |   <= 重启当前服务
	| -------- |
	| Exit     |   <= 停止服务并退出天马伴侣
	+----------+

服务在运行过程中输出的日志信息会通过气泡消息的方式显示，并且会记录在工作目录下的日志文件夹里。

服务在运行过程中如果当前使用的配置文件发生了修改，服务会自动重启，以便让新的配置文件立即生效。

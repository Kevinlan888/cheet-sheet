# lldb 命令
	- platform select remote-android
		远程调试Android应用
	- platform connect connect://:9999
		连接远程调试服务器
	- target create xxx
		设置调试目标 (本地) 用于加载符号
	- env LD_LIBRARY_PATH=/data/local/tmp/dws-sdk
		设置动态库搜索目录
	- platform shell pwd 在
		远程设备上执行pwd命令
	- shell pwd
		在本机执行pwd命令
	- platform process list
		查看远程进程
	- attach [PID]
		附加进程
	- platform settings -w /data/local/tmp/dws-sdk
		设置程序工作目录
	- breakpoint set --file tinyxml.cpp --line 966
		设置断点
	- run
		在远端运行程序, 开始调试
	- next
		在断点时, 运行到下一行
	- step
		在断点时, 进入函数
	- kill
		杀死程序
		
# lldb-server 命令
	- lldb-server p --server --listen 0.0.0.0:9999
		开启调试服务器,并且监听9999端口
		

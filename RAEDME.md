#先运行服务器再另开终端运行客户机
#服务器
#编译
gcc s.c  -L/usr/local/v6/lib -lm -lsctp -o server
#运行，参数2是最大输入流个数，参数3是输出流个数
./server 5 100 10

#客户机
#编译
gcc c.c  -L/usr/local/v6/lib -lm -lsctp -o client
#运行, 参数2是服务端地址，参数3是最大输入流个数，参数4是输出流个数，参数5必须小于参数4
./client 192.168.124.4 100 81 8

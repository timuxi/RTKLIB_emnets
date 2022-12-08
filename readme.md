# 前言
本代码只尝试过在树莓派上使用。且仅使用了consapp下的rtkrcv功能。
# 使用方法
> cd ~/RTKLIB/app/consapp/rtkrcv/gcc

如果需要对代码源码进行了修改，需要重新编译的话，在gcc目录下使用以下命令，就可以完成自动编译。
> make

启动rtklib，进行定位。其中rtkconf.conf是配置文件，串口和网络端口都需要在里面进行配置。
> ./rtkrcv -o ../conf/rtkconf.conf -s

如果出现start success，则表示启动成功。此时可以输入下面命令，来看当前的运行状态。
>status 查看运行状态
>solution 定位结果
>error 如果定位失败，会在里面打印相应的错误日志。可以按control+c退出当前状态。
>stop 停止rtk运行
>shutdown 退出当前的命令行状态

# MAC解决端口占用

## 1.查看端口
终端输入：lsof -i tcp:port 将port换成被占用的端口(如：8086、9998)
将会出现占用端口的进程信息。

## 2.kill进程
找到进程的PID,使用kill命令：kill PID（进程的PID，如2044），杀死对应的进程。
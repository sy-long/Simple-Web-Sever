# 一个简单的Web服务器

## 特性：
* 多进程服务
* 针对僵尸进程进行回收处理
* 针对accept()被打断进行重启处理
* 支持.cgi文件脚本运行
* 支持目录显示
* 支持html等类型文件浏览
* 仅支持GET操作

## 部署测试方法：

* 环境：linux
* 编译：gcc -o web-server.out web-server.c
* 运行：./web-server.out portnum(自定义任意合规端口号) &
* 测试：telnet 0.0.0.0 portnum，然后键入GET filename（文件/目录）
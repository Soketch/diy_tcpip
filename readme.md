###  从0实现一个TCP/IP协议栈
本项目旨在从零开始实现一个TCP/IP协议栈，主要内容包括：

- 网络层：实现IPv4协议，包括IP头部校验、IP分片、IP路由、ARP协议等。
- 传输层：实现TCP协议，包括TCP连接管理、流量控制、拥塞控制、滑动窗口、超时重传等。
- 应用层：实现HTTP协议，包括HTTP请求、响应、Cookie、Session等。
- 网络接口：实现网络接口，包括网卡驱动、网络协议栈、网络设备等。
- 其他：实现网络栈的可靠性和可扩展性，包括多线程、多进程、异步I/O、事件驱动等。


工程配置：
   1. gcc + gdb + cmake


工程目录：
        |--DiyTcpIp
            |
            ├─build
            |   └─构建调试输出目录 build/debug/testbuild
            ├─npcap
            |   └─npcap 开发包
            |
            ├─src   # 源代码目录
            │  ├─app  # 通过net开发的应用程序
            │  ├─net  # 网络协议栈核心源码
            │  └─plat # 平台相关源码        
            |   
            └─work  # 工程相关文件
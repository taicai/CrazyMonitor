# CrazyMonitor

# 项目需求:

1. 同时监控多台服务器的使用情况,比如 CPU,网卡,硬盘等
2. 实现报警功能,希望当某一台服务器的某一个服务达到阈值就触发报警
3. 监控服务器上各个软件的运行状态
 
# 项目架构

由三个部分组成:

服务端:用 django 实现,用来接收客户端上传的数据,并在前台显示
客户端:每个服务器一个客户端,一个客户端会有多个服务,一般一个软件将是一个服务
监控服务:运行在服务端的一个单独的程序,用来监控报警



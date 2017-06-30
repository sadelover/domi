# 安装引擎核心程序

* Gatewaycore  下载地址: [core.rar](http://beop.rnbtech.com.hk/static/help/BEOPGatewayCore_2015_12_18.rar)，本软件为绿色软件，下载后可任意位置放置，建议统一在d:\core目录下，解压即可。
* 将GatewayCore.exe加入系统的启动项中，在开始菜单中在启动上右键-打开，创建快捷方式到Gatewaycore.exe

第一次安装时，.ini里 dbbuild=0

# 启动引擎

* 通过双击GatewayCore.exe即可启动引擎
* 启动后console窗口显示 `engine started successfully`表示启动成功

  ```
    提示：当Gatewaycore引擎启动时，将有看门狗软件BeOPWatch.exe同时自动运行在后台，
    在桌面右下角通知区看到BEOPWatch的图标，通过点击可以看到监视状态。
  ```

# 启动策略引擎

* 通过双击LogicEngine.exe即可启动引擎

# 启动web服务引擎

* 通过命令行 python runEngine.py 即可启动引擎

# 设置开机自启动

* 将dog.exe放入开机启动项中即可




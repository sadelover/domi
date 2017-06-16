#点表文件制作指南#

##第一步：制作点表文件##

1. 制作点表文件（格式为xlsx，需用Microsoft Excel进行编辑），点表模板从[这里](http://beop.rnbtech.com.hk/static/help/pointdebug/opcpointdemo.xlsx)下载。只有完全符合格式要求的点表文件，才能顺利导入到现场组态文件中。
   点表文件由多行构成，除第一行表示题头（不能擅自删除）外，每行表示一个现场的点。目前本平台支持的点类型及对应属性如下表。




注意，`source`列内容必须在上述<b>点来源类型清单</b>中。


这里，提供了常用的一些点表文件范例:

西门子OPC Server 访问点表: [opcpointdemo.xlsx](http://beop.rnbtech.com.hk/static/help/pointdebug/opcpointdemo.xlsx)

##第二步：将点表文件导入至现场引擎Core中##
1. 下载 Factory , 下载地址: [BeOPFactory_2015_12_18.zip](http://beop.rnbtech.com.hk/static/help/BeOPFactory_2015_12_18.zip)
2. 进入Factory，打开组态文件（.s3db），菜单中进入点表管理
3. 导入点表文件
4. 将文件拷贝至core同目录覆盖后，重启core软件（关闭Core控制台窗口即可，系统会自动重启）
5. core软件是控制台软件，运行后的屏幕上会提示错误信息，必须确保窗口的滚动信息内不出现<font color=red><b>`Error`</b></font>字样，才表示通讯正常。常见的一些错误信息如下：


##第三步: 用验证点值##
1. 从Factory菜单`调试` - `启动调试工具`, 实时数据库地址输入引擎盒子的IP地址，登录成功即可进入点调试界面，这里可以辅助查找点值、趋势分析等。
2. `服务器管理`面板中，确认当前模式为`现场`，如果是`仿真`模式下，引擎不会读取现场总线上的真实数据。
2. `点位监控`面板中，可用于监视所读取到的点值
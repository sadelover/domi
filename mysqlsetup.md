下载 **mysql-essential-5.1.40-win32.exe **

安装采用默认选项，不断Next，注意在配置Instance时需要将端口加入到防火墙意外中，如下图：

![](/assets/2017-06-13_191414.png)

编码选择采用utf8，如下：

![](file:///C:/Users/golding/AppData/Local/Temp/msohtmlclip1/01/clip_image001.png "1")

注意加入到环境变量：

![](file:///C:/Users/golding/AppData/Local/Temp/msohtmlclip1/01/clip_image001.png "1")

创建root用户和密码，注意密码必须为指定的通用数据库密码（密码向产品经理索取）

![](file:///C:/Users/golding/AppData/Local/Temp/msohtmlclip1/01/clip_image001.png)

MySQL安装完后，右键计算机-&gt;管理，选择服务与应用程序-&gt;服务，找到MySQL服务，右键停止服务。

打开MySQL安装目录，打开my.inf配置文件。（NotePad++打开）

找到下列三个变量（找不到则添加），修改数值

innodb\_file\_per\_table=1//1个表对应一个

tmp\_table\_size=128M//内存表容量设置  
max\_heap\_table\_size=128M

找到下列三个变量，查看是否满足条件。

default-character-set=utf8//字符集

basedir="D:/Program Files/MySQL/MySQL Server 5.1/"//安装地址

datadir="D:/ProgramData/MySQL/MySQL Server 5.1/Data/"//数据存放地址（不要放系统盘）

修改保存后，重新打开

MySQL

服务（右键计算机

-

&gt;

管理，选择服务与应用程序

-

&gt;

服务，找到

MySQL

服务，右键启动服务）。


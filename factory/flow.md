# **绘制界面指南**

1、新建项目

打开factory软件，点击工具栏中的新建项目，在弹出设置框中，会有如下选项：

项目名称：使用英文字符、数字、下划线

存放位置：通过右侧...按钮点击选择存放位置

设备类型：默认选项即可

点击确定。

注意：如果存放位置为空，项目会自动保存在factory的根目录下。

2、创建页面

factory中的页面通过组的形式管理，因此在创建页面前需要创建一个组：在左侧栏框点击页面，单击右键选择增加组，在弹出的对话框中输入组名称后，点击确定。

选择组，单击右键选择增加页，弹出如下对话框：

![](/assets/新建页面.png)

画面名称：尽可能描述新建页面的界面内容，如：机房、冷却塔操作界面等

界面类型：

```
             固定页面（固定于界面上的页面）

             浮动页面（通过图元链接所跳转的页面 ）

             网站页面

 当选择固定页面时，勾选Observer是否制定，可在Observer内看到该页面操作状态，否则不需要勾选。
```

画面大小：

```
             当选择固定页面时，画面大小为默认；

            当选择浮动页面时，画面大小可以自行调整。
```

背景图：

```
           可根据需要选择，一般不需要使用背景图，不用勾选。
```

点击确定，即可成功地创建一个页面。

3、绘制界面

在工具栏上可以选择不同的功能按钮来插入不同的功能。  
目前可以实现的功能有：管道、直线、矩形、圆形、文本框、冷机图、水泵图、阀门图、冷却塔图、通用图元、按钮、弯管图、仪表盘、折线图、柱状图、饼图、时间选择空间、时间序列图、进度条、折线诊断图、点阵诊断图等。

以下仅介绍通用图元和文本框的插入方法。

3.1插入通用图元

点击工具栏上的自定义图元按钮，再点击组态界面，即会弹出图元选择窗口。![](/assets/图元按钮.png)![](/assets/图元选择窗口.png)如需导入图元，点击：功能/导入图元，即可在我的电脑中选择PNG图片加入到图元库中。  
在图元窗口中选择合适的图元后，双击，即可将选中图元添加到组态界面上。

如需导入动画，点击：界面/动画，即可切换到动画界面，再点击：功能/导入动画，即可在我的电脑中选择PNG序列图片加入到图元库中。

3.2图元自定义设置

在插入图元后，双击该图元，可对其进行设置，如图：

![](/assets/图元链接1.png)

图元名称：自定义

图层：层数由低到高显示

状态定义：主要是绑定点位 （在绑定点位内有详细描述）

事件定义：用于定义该图元的事件类型 （在图元链接内有详细描述）

3.2插入文本框

点击工具栏上的文本框按钮，再点击组态界面，即可添加文本框。

双击文本框，即可出现文本框编辑的对话框。

![](/assets/文本框编辑.png)

其中，  
默认文本：编辑文本框的默认显示信息。  
字体：设定字体  
字体颜色：设定字体颜色  
字体大小：设定字体大小  
对齐：设定文字对齐方式  
边框：功能暂无  
边框背景：功能暂无  
层：设定字符串的图层层数，图层一共有10层。其中1层最低，10层最高。高层图元会覆盖低层图元。

显示类型：  
显示类型分为值模式和枚举模式。  
选为值模式时直接显示点位数值  
枚举模式需要进行配置，如：0:关闭\|1:开启。表示当值为0时，显示“关闭”，当值为1时，显示“开启”。

小数位数：设定值模式时点位的小数位数。

4、图形的对齐

在工具栏上左端是对齐功能，可实现图元的左对齐、右对齐、上对齐、下对齐、横向等间距、纵向等间距、等大处理等对齐功能。

![](/assets/图形对齐按钮.png)

操作方法：  
点击鼠标图案选中要对齐的图元，按住ctrl再选择第二个图元，进行复选，选择完毕后，点击所需要的对齐按钮即可。


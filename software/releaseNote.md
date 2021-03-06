### COPYRIGHT
THE INFORMATION CONTAINED HERE IS PROPRIETARY TECHNICAL 
INFORMATION OF FOHEART CO., LTD. TRANSMITTING, REPRODUCTION, 
DISSEMINATION AND EDITING OF THIS DOCUMENT AS WELL AS 
UTILIZATION OF THE CONTENT ARE FORBIDDEN WITHOUT PERMISSION. 
OFFENDERS WILL BE HELD LIABLE FOR PAYMENT OF DAMAGES. ALL 
RIGHTS ARE RESERVED IN THE EVENT OF A PATENT GRANT OR 
REGISTRATION OF A UTILITY MODEL OR DESIGN.
### GENERAL NOTES
FOHEART OFFERS THE INFORMATION AS A SERVICE TO ITS CUSTOMERS. 
THE INFORMATION PROVIDED IS BASED UPON CUSTOMERS’ 
REQUIREMENTS. FOHEART MAKES EVERY EFFORT TO ENSURE THE 
QUALITY OF THE INFORMATION IT MAKES AVAILABLE. FOHEART DOES 
NOT MAKE ANY WARRANTY AS TO THE INFORMATION CONTAINED 
HEREIN, AND DOES NOT ACCEPT ANY LIABILITY FOR ANY INJURY, LOSS 
OR DAMAGE OF ANY KIND INCURRED BY USE OF OR RELIANCE UPON 
THE INFORMATION. ALL INFORMATION SUPPLIED HEREIN IS SUBJECT TO 
CHANGE WITHOUT PRIOR NOTICE.<br>
**For technical support, please visit:**<br>
[http://www.foheart.com/support.html](http://www.foheart.com/support.html) or<br>
[http://www.foheart.com/question.html](http://www.foheart.com/question.html)<br>
**北京总部**<br>
Tel：(+86)010-56106165<br>
Email：contact@foheart.com<br>
地址：北京市海淀区黑山扈路红山口8号D2-南-3号<br>
邮编：100091<br>

<div align=center>
<img src="https://raw.githubusercontent.com/FOHEART/FOHEART_Unity3D_Plugin/master/help/img/address1.png"/>
</div>

**Copyright(C) FOHEART Co., Ltd. 2015-2018. All rights reserved.**<br>

----------
[MotionVenus 1.4.0]<br>
1. 姿态解算性能优化。
2. 软件主页面优化。
3. 用户配置保留功能。
4. 自定义动画库路径/.RAW文件关联等功能。
5. bug及细节优化。
视频介绍地址：
http://www.foheart.com/experience.html或http://i.youku.com/foheart
----------
[MotionVenus 1.3.8]<br>
1. 姿态解算能够自动处理大部分上下跳动、滑动等问题。
2. 增加了文件打包功能，便于将动捕文件快速复制到任意位置。
3. 增加了原始数据导出功能，详见博客http://blog.foheart.com/。
4. bug及细节优化。
5. 本软件手册地址(Github)：[https://github.com/FOHEART/MotionVenusHelp/tree/v1.3.8](https://github.com/FOHEART/MotionVenusHelp/tree/v1.3.8)<br>
视频介绍地址：[http://www.foheart.com/experience.html](http://www.foheart.com/experience.html)<br>或<br>[http://i.youku.com/foheart](http://i.youku.com/foheart)
----------
[MotionVenus 1.3.6]<br>
1. 修正了bvh导出数据帧数不正确的问题。
2. 内置Unroll与Gimble修复机制，直接导出正确的fbx，无需在MotionBuilder中进行修正。
3. 增加了使用游戏引擎控制MotionVenus功能，详见应用手册AN3363([http://blog.foheart.com/?p=66](http://blog.foheart.com/?p=66))。
4. bug及细节优化。

--------------------
[MotionVenus 1.3.4]<br>
1. 增加节点受到严重磁干扰后的明显视觉提示。
2. 增加录制文件夹的自动监控功能，文件增删后列表会自动更新。
3. 修正了检测路由器和充电底座数目不正确的问题。
4. 增加了软件自动更新功能，请在帮助->检查更新中检查是否有新版本。
5. 修正了网络数据流中位移数据微小差异的问题（此问题会影响Unity3D、UE4及MotionVenusSDK）。
6. 节点校准界面为每个节点都增加了单独校准的按钮。
7. 优化了算法，节点校准的速度及成功率更高了。
8. 修改了非整数帧率播放bug。
9. 修改了UDP发送配置中四元数、欧拉角的旋转顺序无效的问题。
10. 数十项bug及细节优化。

----------

[MotionVenus 1.3.2]<br>
1. 增加了UDP转发动作数据流的字符串格式。
2. 增加了UDP转发动作数据流的骨骼旋转模式，现在可以选择发送骨骼本地旋转或全局旋转。
3. 解决了打开回放文件再连接设备的崩溃问题。
4. 添加右下角上线套装个数显示。
5. 其它bug修复。

----------

[MotionVenus 1.3.0 SP1]
1. 增加了BVH直接导出到3Ds Max中的Biped BVH格式。
2. 完整支持所有电影、电视播放及导出的帧率选择，添加例如PAL、NTSC等制式的支持。
3. 增加了录制动画时，主窗体边框红色闪烁状态提示。
4. 修正了导出的fbx不兼容3Ds Max 2016之前版本的问题。
5. 修正了接触点编辑导致的闪退问题。
6. 大量细节优化。

----------

[MotionVenus 1.3.0]
1. 增加了离线数据的网络发送，最多支持五组，可在Unity3D、UE4中播放多人离线数据流。
2. 修改网络数据发送为后台自动转发。
3. 增加了RAW文件的详情页，可查看文件内部信息。
4. 增加了绘图区欧拉角旋转顺序设置，支持所有六种旋转顺序。
5. 增加了多语言切换，现已支持英文。
6. 增加了交互性帮助功能，单击每个组件右上角的问号按钮，可获得与本组件相关的网络帮助文档。
7. 增加了节点校准视频。
8. 其它细节bug修正。

----------

[MotionVenus 1.2.8]
1. 增加了数据帧修改模块，可以修正轻微的滑步抖动。
2. 更新了转发到游戏引擎的数据流格式。
3. 统一了导出BVH中所有骨骼的坐标系方向。
4. 修正了多套套装同时连接左侧设备列表显示的问题。
5. U3D与UE4的使用demo和文档请到[http://www.foheart.com/resource.html](http://www.foheart.com/resource.html)下载使用。

----------

[MotionVenus 1.2.1]
1. 更新了骨骼姿态解算算法。
2. 修改骨骼长度的bug修复。
3. 部分已知bug的修复。

<div align=center>
<img src="https://raw.githubusercontent.com/FOHEART/FOHEART_Unity3D_Plugin/master/help/img/tail.png" width="100%"/>
</div>
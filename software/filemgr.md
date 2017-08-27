## 4.8 录制文件管理

录制文件管理模块主要负责：
1. 存储、管理、回放录制的动捕文件；
2. 导出动作文件为BVH、FBX等通用格式；

<div align=center>
<img src="https://raw.githubusercontent.com/FOHEART/MotionVenusHelp/v1.3.0/software/filemgr.png"/>
</div>

文件命名规则：录制日期+时间+角色名。<br>
如20170713_172853_Actor1(Live)，20170713代表录制的时间2017年7月13日，_172853代表录制时间17点28分53秒，_Actor1(Live)代表实时角色名；<br>
3. 右键已打开的文件，在弹出菜单中选择“导出时间轴范围内数据”，导出数据为时间轴模块中间两个滑块确定的范围。

<div align=center>
<img src="https://raw.githubusercontent.com/FOHEART/MotionVenusHelp/v1.3.0/software/fileexport.png"/>
</div>

4. 右键选择属性，查看录制文件的详细信息，包括使用的硬件套装、总帧数、骨骼长度等信息。

<div align=center>
<img src="https://raw.githubusercontent.com/FOHEART/MotionVenusHelp/v1.3.0/software/filemgrprop.png"/>
</div>

5. 右键选择添加到播放队列，是指将当前文件添加到回放流中，所有在播放列表中的文件，均会在后台转发其数据到网络端口（例如发送到Unity3D、Unreal Engine 4等第三方软件中）。
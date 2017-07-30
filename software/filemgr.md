## 4.8 录制文件管理

录制文件管理模块主要负责：
1. 存储、管理、回放录制的动捕文件；
2. 导出动作文件为BVH、FBX等通用格式。
<div align=center>
<img src="https://raw.githubusercontent.com/FOHEART/MotionVenusHelp/master/software/filemgr.png"/>
</div>
文件命名规则：录制日期+时间+角色名。<br>
如20170713_172853_Actor1(Live)，20170713代表录制的时间2017年7月13日，_172853代表录制时间17点28分53秒，_Actor1(Live)代表实时角色1。
3. **右键**已打开的文件，在弹出菜单中选择“导出时间轴范围内数据”，导出数据为[时间轴模块](https://github.com/FOHEART/MotionVenusHelp/blob/master/software/timeline.md)中间左右两个滑块确定的范围。
<div align=center>
<img src="https://raw.githubusercontent.com/FOHEART/MotionVenusHelp/master/software/fileexport.png"/>
</div>
## 4.7 时间轴
时间轴栏主要用来管理实时数据的录制、回放、快速慢速播放、配合帧数据修改模块修改数据等功能。

<div align=center>
<img src="https://raw.githubusercontent.com/FOHEART/MotionVenusHelp/v1.3.2/software/timeline.png"/>
</div>

1. 点击**录制按钮**录制实时数据流，录制完成的数据流会显示在录制文件管理模块中。

录制时主窗体会用红色边框标红：

<div align=center>
<img src="https://raw.githubusercontent.com/FOHEART/MotionVenusHelp/v1.3.2/software/recordredhint.png"/>
</div>

注意在录制时，**无法回放同时回放文件**，如果切换到回放模式，会造成录制内容为**空白**。

2. 回放帧率可更改，用来**预览**以此帧率导出为BVH或FBX后的实际效果。
帧率选择现已支持所有制式帧率。

<div align=center>
<table>
    <tr><th>帧率</th><th>备注</th></tr>
    <tr><th>23.976 fps</th><th></th></tr>
    <tr><th>24fps</th><th></th></tr>
    <tr><th>PAL</th><th>25 fps</th></tr>
    <tr><th>NTSC Full</th><th>29.97 fps</th></tr>
    <tr><th>NTSC Drop</th><th>29.97 fps</th></tr>
    <tr><th>30 fps</th><th></th></tr>
    <tr><th>48 fps</th><th></th></tr>
    <tr><th>59.94 fps</th><th></th></tr>
    <tr><th>72 fps</th><th></th></tr>
    <tr><th>96 fps</th><th></th></tr>
    <tr><th>100 fps</th><th></th></tr>
    <tr><th>120 fps</th><th></th></tr>
    <tr><th>1000 fps</th><th></th></tr>
</table>
</div>

3. 中间左右两个滑块用来控制时间轴**显示的区域**。

<div align=center>
<img src="https://raw.githubusercontent.com/FOHEART/MotionVenusHelp/v1.3.2/software/timelinemedium.GIF"/>
</div>

可以直接双击滑块输入帧号实现快速跳转。

<div align=center>
<img src="https://raw.githubusercontent.com/FOHEART/MotionVenusHelp/v1.3.2/software/timelinedinputmedium.GIF"/>
</div>

4. 播放模式有四种：
 
> “正常播放”；
> “按帧拖动”播放为拖动时间轴滑块时，**最小间隔**为一帧；
> “按帧播放”为播放时**最小间隔**为一帧；
> “按帧拖动播放”为播放及拖动时，**最小间隔**均为一帧。

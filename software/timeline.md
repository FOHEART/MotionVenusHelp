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
<img src="https://raw.githubusercontent.com/FOHEART/FOHEART_Unity3D_Plugin/master/help/img/address1.png"  width="100%"/>
</div>

**Copyright(C) FOHEART Co., Ltd. 2015-2018. All rights reserved.**<br>

## 4.7 时间轴
时间轴栏主要用来管理实时数据的录制、回放、快速慢速播放、配合帧数据修改模块修改数据等功能。

<div align=center>
<img src="https://raw.githubusercontent.com/FOHEART/MotionVenusHelp/v1.3.4/software/timeline.png" width="100%"/>
</div>

1. 点击**录制按钮**录制实时数据流，录制完成的数据流会显示在录制文件管理模块中。

录制时主窗体会用红色边框标红：

<div align=center>
<img src="https://raw.githubusercontent.com/FOHEART/MotionVenusHelp/v1.3.4/software/recordredhint.png" width="100%"/>
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
<img src="https://raw.githubusercontent.com/FOHEART/MotionVenusHelp/v1.3.4/software/timelinemedium.GIF" width="100%"/>
</div>

可以直接双击滑块输入帧号实现快速跳转。

<div align=center>
<img src="https://raw.githubusercontent.com/FOHEART/MotionVenusHelp/v1.3.4/software/timelinedinputmedium.GIF" width="100%"/>
</div>

4. 播放模式有四种：
 
> “正常播放”；
> “按帧拖动”播放为拖动时间轴滑块时，**最小间隔**为一帧；
> “按帧播放”为播放时**最小间隔**为一帧；
> “按帧拖动播放”为播放及拖动时，**最小间隔**均为一帧。

<div align=center>
<img src="https://raw.githubusercontent.com/FOHEART/FOHEART_Unity3D_Plugin/master/help/img/tail.png" width="100%"/>
</div>
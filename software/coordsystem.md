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

## 6.1 坐标系定义
### 6.1.1 硬件坐标系定义
硬件指惯性动作捕捉节点（IMU Sensor），其坐标系定义如下：

<div align=center>
<img src="https://raw.githubusercontent.com/FOHEART/MotionVenusHelp/v1.4.2/software/sensorcoord.png" />
</div>

导光柱指向y轴，右侧指向x轴，z轴指向Sensor正上方。<br>

符合该坐标系的输出值：<br>
17个Sensor加速度值、角速度值。
### 6.1.2 四元数、欧拉角坐标系定义
符合东(X)北(Y)天(Z)坐标系定义。<br>
符合该坐标系的输出值：<br>
在MotionVenus中直接拖拽设备列表中的某个Sensor到绘图区窗口，显示的实时曲线值。
### 6.1.3 MotionVenus骨骼坐标系定义
符合右手坐标系定义。<br>
<div align=center>
<img src="https://raw.githubusercontent.com/FOHEART/MotionVenusHelp/v1.4.2/software/skeletoncoord.png"  width="100%"/>
</div>

如上图所示，世界坐标系为右手坐标系，T-Pose时每段骨骼的local及global坐标系也均为右手坐标系。<br>
每段骨骼在T-Pose时角度定义为（0,0,0）。<br>
可以输出每段骨骼的本地（Local）旋转值或者全局（Global）旋转值。<br>
符合该坐标系的输出值：<br>
23段骨骼旋转角度、22个关节旋转角度。
## 6.2 Unity3D坐标系
摘录自[[链接]](https://blog.csdn.net/biezhihua/article/details/77489399)<br>

<div align=center>
<img src="https://raw.githubusercontent.com/FOHEART/MotionVenusHelp/v1.4.2/software/Cartesian_coordinate_system_handedness.png"/>
</div>

<div align=center>
<img src="https://raw.githubusercontent.com/FOHEART/MotionVenusHelp/v1.4.2/software/leftrighthand.png"/>
</div>

3D坐标系是3D游戏开发的基础概念。一般3D软件都是采用笛卡尔坐标系来描述物体的坐标信息。笛卡尔坐标系分为左手坐标系和右手坐标系：<br>

左手坐标系是Y轴指向上方，X轴指向右方，Z轴指向前方。<br>
右手坐标系是Y轴指向上方，X轴指向右方，Z轴指向后方。<br>
在Unity3D中使用的是左手坐标系，其中X轴代表水平方向，Y轴代表垂直方向，而Z轴代表深度。<br>
在MotionVenus中使用的是右手坐标系，其中X轴代表水平方向，Z轴代表垂直方向，而Y轴代表深度。<br>

<div align=center>
<img src="https://raw.githubusercontent.com/FOHEART/FOHEART_Unity3D_Plugin/master/help/img/tail.png" width="100%"/>
</div>
## 6.1 坐标系定义
### 6.1.1 硬件坐标系定义
硬件指惯性动作捕捉节点（IMU Sensor），其坐标系定义如下：

<div align=center>
<img src="https://raw.githubusercontent.com/FOHEART/MotionVenusHelp/v1.4.0/software/sensorcoord.png"/>
</div>

导光柱指向y轴，右侧指向x轴，z轴指向Sensor正上方。<br>

符合该坐标系的输出值：<br>
17个Sensor加速度值、角速度值。
### 6.1.2 四元数、欧拉角坐标系定义
符合东(X)北(Y)天(Z)坐标系定义。<br>
符合该坐标系的输出值：<br>
在MotionVenus中直接拖拽设备列表中的某个Sensor到绘图区窗口，显示的实时曲线值。
### 6.1.3 骨骼坐标系定义
符合右手坐标系定义。<br>
<div align=center>
<img src="https://raw.githubusercontent.com/FOHEART/MotionVenusHelp/v1.4.0/software/skeletoncoord.png"/>
</div>

如上图所示，世界坐标系为右手坐标系，T-Pose时每段骨骼的local及global坐标系也均为右手坐标系。<br>
每段骨骼在T-Pose时角度定义为（0,0,0）。<br>
可以输出每段骨骼的本地（Local）旋转值或者全局（Global）旋转值。<br>
符合该坐标系的输出值：<br>
23段骨骼旋转角度、22个关节旋转角度。
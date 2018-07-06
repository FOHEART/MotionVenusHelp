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

## 4.8 库

### 1、功能概述
库模块主要负责：
1. 存储、管理、回放录制的动捕文件；
2. 导出动作文件为BVH、FBX等通用格式；

<div align=center>
<img src="https://raw.githubusercontent.com/FOHEART/MotionVenusHelp/v1.4.2/software/filemgr.png"/>
</div>

文件命名规则：录制日期+时间+角色名。<br>
如20170713_172853_Actor1(Live)，20170713代表录制的时间2017年7月13日，_172853代表录制时间17点28分53秒，_Actor1(Live)代表实时角色名；<br>
### 2、数据导出
右键已打开的文件，在弹出菜单中选择“导出时间轴范围内数据”，导出数据为时间轴模块中间两个滑块确定的范围。

<div align=center>
<img src="https://raw.githubusercontent.com/FOHEART/MotionVenusHelp/v1.4.2/software/fileexport.png"/>
</div>

1. 导出选项

对于同名文件的处理，有三种选择：
- 自动重命名：会自动在重名文件后添加"_1"后缀。
- 覆盖：自动覆盖重名文件。
- 询问：每次都弹出对话框询问是否覆盖。

自动添加biped后缀为当导出文件为3Ds Max Biped BVH时，在文件末尾自动添加_biped后缀。<br>
2. 帧率选择

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

### 3、3Ds Max Biped BVH
导出格式选择3Ds Max Biped BVH：

<div align=center>
<img src="https://raw.githubusercontent.com/FOHEART/MotionVenusHelp/v1.4.2/software/bipedbvhexport.png"  width="100%"/>
</div>

在3Ds Max中可以直接支持导入该种文件格式，使用方法为：<br>
首先在场景中拖拽创建出一个默认的Biped模型，

<div align=center>
<img src="https://raw.githubusercontent.com/FOHEART/MotionVenusHelp/v1.4.2/software/bipedbvhcreate.png"  width="100%"/>
</div>

然后选择Load Motion Capture File，

<div align=center>
<img src="https://raw.githubusercontent.com/FOHEART/MotionVenusHelp/v1.4.2/software/bipedbvhload.png"  width="100%"/>
</div>

选择刚才导出的ActorM_biped.bvh即可，最终显示如下：

<div align=center>
<img src="https://raw.githubusercontent.com/FOHEART/MotionVenusHelp/v1.4.2/software/bipedbvhimport.png"  width="100%"/>
</div>

### 4、FBX导出
FBX导出与BVH导出步骤完全相同，选择：<br>
1. 起始帧、结束帧。
2. 导出帧率。
3. 点击导出。

### 5、文件信息
1. 右键选择属性，查看录制文件的详细信息，包括使用的硬件套装、总帧数、骨骼长度等信息。

<div align=center>
<img src="https://raw.githubusercontent.com/FOHEART/MotionVenusHelp/v1.4.2/software/filemgrprop.png"/>
</div>

### 6、播放列表
1. 右键选择添加到播放队列，是指将当前文件添加到回放流中，所有在播放列表中的文件，均会在后台转发其数据到网络端口（例如发送到Unity3D、Unreal Engine 4等第三方软件或引擎中）。

### 7、文件打包
当需要在不同存储位置移动动捕文件时，为了方便操作，可以使用MotionVenus内置的文件打包功能，快速压缩当前文件及其所有相关文件到指定存储位置。<br>
在"库"停靠栏中，选择需要操作的文件，右键选择"打包文件"，弹出以下菜单：

<div align=center>
<img src="https://raw.githubusercontent.com/FOHEART/MotionVenusHelp/v1.4.2/software/filecompress.png"/>
</div>

RAW文件：动捕数据原始文件。<br>
TRE文件：保存了接触点编辑的信息，如果编辑过接触点，建议勾选此项。<br>
CSV文件：保存了Sensor的原始数据（四元数、欧拉角、加速度、角速度、磁力值）信息，如果在录制时在设置中打开了原始数据导出选项，则会产生此文件。<br>
AVI文件：保存了同步视频录像，如果在动捕过程中使用了摄像头捕捉功能，则会产生同步录像文件。<br>

压缩后生成以文件名命名的.zip文件。<br>
如果需要使用打包后的动捕文件，需要将其解压到MotionVenus的库文件夹根目录中。

<div align=center>
<img src="https://raw.githubusercontent.com/FOHEART/FOHEART_Unity3D_Plugin/master/help/img/tail.png" width="100%"/>
</div>
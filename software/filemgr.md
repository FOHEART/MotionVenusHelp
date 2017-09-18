## 4.8 录制文件管理

### 1、功能概述
录制文件管理模块主要负责：
1. 存储、管理、回放录制的动捕文件；
2. 导出动作文件为BVH、FBX等通用格式；

<div align=center>
<img src="https://raw.githubusercontent.com/FOHEART/MotionVenusHelp/v1.3.0/software/filemgr.png"/>
</div>

文件命名规则：录制日期+时间+角色名。<br>
如20170713_172853_Actor1(Live)，20170713代表录制的时间2017年7月13日，_172853代表录制时间17点28分53秒，_Actor1(Live)代表实时角色名；<br>
### 2、数据导出
右键已打开的文件，在弹出菜单中选择“导出时间轴范围内数据”，导出数据为时间轴模块中间两个滑块确定的范围。

<div align=center>
<img src="https://raw.githubusercontent.com/FOHEART/MotionVenusHelp/v1.3.0/software/fileexport.png"/>
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

3. 3Ds Max Biped BVH
导出格式选择3Ds Max Biped BVH：

<div align=center>
<img src="https://raw.githubusercontent.com/FOHEART/MotionVenusHelp/v1.3.0/software/bipedbvhexport.png"/>
</div>

在3Ds Max中可以直接支持导入该种文件格式，使用方法为：<br>
首先在场景中拖拽创建出一个默认的Biped模型，

<div align=center>
<img src="https://raw.githubusercontent.com/FOHEART/MotionVenusHelp/v1.3.0/software/bipedbvhcreate.png"/>
</div>

然后选择Load Motion Capture File，

<div align=center>
<img src="https://raw.githubusercontent.com/FOHEART/MotionVenusHelp/v1.3.0/software/bipedbvhload.png"/>
</div>

选择刚才导出的ActorM_biped.bvh即可，最终显示如下：

<div align=center>
<img src="https://raw.githubusercontent.com/FOHEART/MotionVenusHelp/v1.3.0/software/bipedbvhimport.png"/>
</div>

4. FBX导出
FBX导出后胳膊或者腿部会有万向锁的产生，会造成错误的瞬间翻转等问题，需要使用MotionBuilder 2014进行数据修复（Plot）。
1. **输入帧数**，选择Plot All

<div align=center>
<img src="https://raw.githubusercontent.com/FOHEART/MotionVenusHelp/v1.3.0/software/fbxplot.png"/>
</div>

2. 配置参数，点击确定

<div align=center>
<img src="https://raw.githubusercontent.com/FOHEART/MotionVenusHelp/v1.3.0/software/fbxplotprop.png"/>
</div>

3. 保存文件退出

### 3、文件信息
1. 右键选择属性，查看录制文件的详细信息，包括使用的硬件套装、总帧数、骨骼长度等信息。

<div align=center>
<img src="https://raw.githubusercontent.com/FOHEART/MotionVenusHelp/v1.3.0/software/filemgrprop.png"/>
</div>

### 4、播放列表
1. 右键选择添加到播放队列，是指将当前文件添加到回放流中，所有在播放列表中的文件，均会在后台转发其数据到网络端口（例如发送到Unity3D、Unreal Engine 4等第三方软件中）。
## 4.10 同步视频捕捉

### 1、功能概述
MotionVenus可以使用USB摄像头同步录制视频流，视频流与动捕数据可以做到帧级别（16.67ms）同步。<br>
使用准备：
1. 能够与系统兼容的USB摄像头。
2. 确保已经正确安装摄像头驱动程序。
在MotionVenus的右侧停靠栏，选择摄像头捕捉，点击刷新按钮获取已连接的摄像头。如果系统中存在多个摄像头，可以在下拉列表中选择需要使用的摄像头设备。

如果有打开的USB摄像头设备，则在点击录制动捕文件时，后台默认同步录制来自摄像头的视频流，录制结束后，视频保存为后缀为.avi的同名视频文件。<br>

视频回放时，如果存在同名的视频文件，则自动在视频窗口同步回放视频文件。<br>

<div align=center>
<img src="https://raw.githubusercontent.com/FOHEART/MotionVenusHelp/v1.4.0/software/cameracapture.png"/>
</div>

视频录制参数：
1. 分辨率：640 x 480px
2. 帧率：30fps
3. 同时录制的视频个数：1个
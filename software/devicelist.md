# 四、软件功能区
## 4.1 设备列表栏

<div align=center>
<img src="https://raw.githubusercontent.com/FOHEART/MotionVenusHelp/v1.3.4/software/devicelist.png"/>
</div>

连接到电脑端的每套设备加载为一个树状列表，树状列表详细的显示了每一个Sensor的连接状态，磁干扰状态和剩余电量。<br>
在[录制文件管理](https://github.com/FOHEART/MotionVenusHelp/blob/v1.3.4/software/filemgr.md)窗体中打开的文件会显示在这里，不同的是回放的文件，无法显示设备信息，只在电量栏中显示“RePlay”字样。

<div align=center>
<img src="https://raw.githubusercontent.com/FOHEART/MotionVenusHelp/v1.3.4/software/devicelistmultireplay.png"/>
</div>

<div align=center>
<table>
   <tr><th>编号</th><th>部位</th><th>部位</th></tr>
   <tr><th>0</th><th>胯部</th><th>Pelvis</th></tr>
	<tr><th>1</th><th>后背</th><th>T8</th></tr>
	<tr><th>2</th><th>头部</th><th>Head</th></tr>
	<tr><th>3</th><th>左肩</th><th>LeftShoulder</th></tr>
	<tr><th>4</th><th>左上臂</th><th>LeftUpperArm</th></tr>
	<tr><th>5</th><th>左小臂</th><th>LeftForeArm</th></tr>
	<tr><th>6</th><th>左手</th><th>LeftHand</th></tr>
	<tr><th>7</th><th>右肩</th><th>RightShoulder</th></tr>
	<tr><th>8</th><th>右上臂</th><th>RightUpperArm</th></tr>
	<tr><th>9</th><th>右小臂</th><th>RightForeArm</th></tr>
	<tr><th>10</th><th>右手</th><th>RightHand</th></tr>
	<tr><th>11</th><th>左大腿</th><th>LeftUpperLeg</th></tr>
	<tr><th>12</th><th>左小腿</th><th>LeftLowerLeg</th></tr>
	<tr><th>13</th><th>左脚</th><th>LeftFoot</th></tr>
	<tr><th>14</th><th>右大腿</th><th>RightUpperLeg</th></tr>
	<tr><th>15</th><th>右小腿</th><th>RightLowerLeg</th></tr>
	<tr><th>16</th><th>右脚</th><th>RightFoot</th></tr>
</table>
</div>

当MotionVenus同时连接多套设备时，系统为设备自动编号，例如Actor1(Live)、Actor2(Live)、Actor3(Live)...，您可以用鼠标点击表头“Actor1(Live)”,点击后表明你所选中了此套设备，接下来的操作都是针对选中的这套设备。<br>
1. “部位”即为这套设备传感器节点所对应的人体部位。
2. “连接”为![noLink](https://raw.githubusercontent.com/FOHEART/MotionVenusHelp/v1.3.4/software/nodeNotLinked.png)时表明这个部位的传感器没有连接上软件，请你检查此传感器是否正常开启，当显示为![noLink](https://raw.githubusercontent.com/FOHEART/MotionVenusHelp/v1.3.4/software/nodeLinked.png)时表明此部位传感器正常连接。
3. “磁干扰”显示为![noMagDisturb](https://raw.githubusercontent.com/FOHEART/MotionVenusHelp/v1.3.4/software/notInMagnetic.png)时表明此部位传感器没有受到周围环境的磁干扰，显示![magDisturb](https://raw.githubusercontent.com/FOHEART/MotionVenusHelp/v1.3.4/software/inMagnetic.png)表明受到了**周围环境的磁干扰**；<br>

本版本新增明显的磁干扰视觉提示，这样即使在距离软件较远的距离，也能看到某个部位受到磁干扰。<br>

![magDisturb](https://raw.githubusercontent.com/FOHEART/MotionVenusHelp/v1.3.4/software/inMagneticHint.png)

4. “电量”则显示了对应部位传感器节点的电量，电量的显示每10秒刷新一次。<br>
**注意**：在使用过程中，由于脚部最容易受到磁干扰，所以当磁干扰一栏显示异常时，应检查周围是否有强磁干扰源，如有应远离，当**远离磁干扰**后，脚部Sensor可以自动恢复正常状态。
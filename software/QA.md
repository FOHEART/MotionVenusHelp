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

# 第五部分：常见问题
## 5.1 软件使用问题
1. Q：为什么动画录制功能无法使用？<br>
   A：MotionVenus的安装目录若在系统盘C盘，则需以**管理员模式**运行，否则无法执行数据录制的操作。软件安装在非系统盘则不存在此问题。
2. Q：为什么多套设备同时使用时，只有一套设备可以显示运动动画？<br>
   A：多套设备同时使用时，应分别校准每套设备，点击选择左侧列表中的设备根节点，在右侧点击校准按钮进行N-Pose、T-Pose等校准流程。
3. Q：安装驱动时总提示“安装失败”？ <br>
   A：有可能是已经安装成功了，只是状态没有更新；请注意一定要将设备驱动放在英文路径下；安装完驱动尝试重启计算机或重新插拔FOHEART C1路由器。
4. Q：单个Sensor的校准是否也可以在游戏引擎中进行？<br>
   A：不可以。现阶段在游戏引擎只支持人体级别的初始动作校准。
5. Q：若使用游戏引擎控制人物校准，MotionVenus是否可以不运行？<br>
   A：不可以。MotionVenus需要运行以解算人体动作。
6. Q：为什么在Unity端点击校准后MotionVenus端无反应？<br>
   A：请检查Unity端人物名称是否填写正确。检查Unity端UDP_Target_IP与UDP_Target_Port是否填写正确。<br>

## 5.2 设备使用问题
1. Q：磁干扰源存在哪些？<br>
   A：节点校准及使用时，应远离磁干扰，例如手机、智能手表、铁、钴、镍以及它们组成的合金等磁体。<br>
磁干扰不限于硬磁软磁等可见实体，大功率变电站、无线基站、空调机柜、或大功率电机等工作时周围数米之内都有极强的磁场干扰。
2. Q：FOHEART C1可同时支持多少套设备同场景使用？<br>
   A：可以在一个软件中同时支持四套设备使用。
3. Q：使用过程中脚部抖动。<br>
   A：远离严重的磁场干扰；调整校准栏下方的“身体倾斜角度值”（从默认值6°开始逐渐加大），逐渐增大或减小找到适合自己的角度。（由于不同人体的腿部倾斜角度并不相同，所以最好手动调整）
4. Q：软件使用过程中节点突然全部掉线。<br>
   A：很大可能是由于HUB使用了质量低劣的USB线缆，请使用我们提供的原装USB线，或质量上等的Micro USB2.0线缆。另外可能是使用了USB集线器，并且由于USB集线器的供电不足造成的设备掉线，请确定您使用的USB集线器能够提供至少350mA供电电流，或者使用有独立电源供电的USB集线器。
5. Q：系统更新后FOHEART C1 HUB或充电底座无法连接。<br>
   A：通常发生在WIN10系统以上，是驱动问题造成的本现象，请参考：[链接](https://github.com/FOHEART/MotionVenusHelp/blob/v1.4.2/driver/driverinstall.md)中的1.4节进行操作。
6. Q：磁干扰会对动作捕捉造成如何影响？<br>
   A：FOHEART动作捕捉系统节点内置磁干扰屏蔽算法，能够屏蔽突发的磁干扰，例如忽然握住手机；屏蔽过程最长持续30秒，若30秒内无法脱离磁干扰，会对最终的效果造成明显的较差影响。
7. Q：硬件Sensor上传数据的速率？<br>
   A：24~96fps，默认96fps。
8. Q：MotionVenus转发数据流到Unity3D或者Unreal Engine的数据速率？<br>
   A：60fps。
9. Q：MotionVenus转发数据流包含什么数据？<br>
   A：23段骨骼的欧拉角；23段骨骼的四元数；23段骨骼的Local坐标；23段骨骼的Gobal坐标；17个Sensor的加速度计原始值；17个Sensor的陀螺仪原始值；17个Sensor的磁力计原始值；（原始值出厂设置不输出）
10. Q：MotionVenus转发数据流可选的格式？<br>
   A：二进制流（此种方式数据包最小）；可读字符串；Json格式；

## 5.3 注意事项

— 勿在热源（如火或加热器）附近使用或贮存动作捕捉传感器；<br>
— 请使用原厂充电底座充电；<br>
— 勿将动作捕捉传感器投入水中或将其弄湿；<br>
— 勿给动作捕捉传感器加热；<br>
— 禁止撞击、投掷或者使动作捕捉传感器受到机械震动；<br>
— 禁止锤击或脚踏动作捕捉传感器；<br>
— 禁止以任何方式拆解动作捕捉传感器；<br>
— 禁止在火源或极热条件下给动作捕捉传感器充电；<br>
<br>
- 请使用原装适配器给充电底座供电，劣质适配器可能会导致动作捕捉传感器电池损坏。<br>

<div align=center>
<img src="https://raw.githubusercontent.com/FOHEART/FOHEART_Unity3D_Plugin/master/help/img/tail.png" width="100%"/>
</div>

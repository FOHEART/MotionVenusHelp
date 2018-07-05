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
## 4.9 接触点编辑
该模块用来修改动捕过程中偶然发生的错误，例如滑步、抖动等问题。

<div align=center>
<img src="https://raw.githubusercontent.com/FOHEART/MotionVenusHelp/master/software/contacteditor.png"/>
</div>

操作流程：
帧数据修改窗口共有两条数据帧状态展示， 上方为“ LFoot” 表示对于左脚
的状态修正，下方为“ RFoot” ，表示对右脚的状态修正。 在加载完成录制的数据文件后，确定要修改的动画范围，以右键点击位置为起点，拖动到指定位置后抬起为终点，此时会有如下菜单以供算法修正

<div align=center>
<img src="https://raw.githubusercontent.com/FOHEART/MotionVenusHelp/master/software/contactcontext.png"/>
</div>

- 选择 “ 触地” ，算法将选择的数据段执行按当前选择的“LFoot” 或“ RFoot”为着地点运算状态算法，重新解算之后的数据状态。
- 选择 “不触地”， 算法将选择的数据段执行按当前选择的 “LFoot”或 “ RFoot”为非着地点运算状态算法， 重新结算之后的数据状态。
- 选择“默认” ，算法将选择的数据段恢复为最初未修改数据的状态， 并重新进行解算。
编辑完成后，请在文件菜单中选择保存。

<div align=center>
<img src="https://raw.githubusercontent.com/FOHEART/FOHEART_Unity3D_Plugin/master/help/img/tail.png" width="100%"/>
</div>
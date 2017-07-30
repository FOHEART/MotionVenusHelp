## 4.9 接触点编辑
该模块用来修改动捕过程中偶然发生的错误，例如滑步、抖动等问题，这些问题一般是由于运动过于
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

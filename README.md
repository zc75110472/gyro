# gyro
1.有两种Javascript事件负责处理手机的重力感应设备方向信息。 <br>
OrientationChange (在屏幕发生翻转的时候触发) <br>
DeviceOrientation（移动的角度）+DeviceMotion （移动的加速度信息）---重力感应与陀螺仪 <br>
重力感应，基本上是平板电脑和智能手机的标准配置，起到的作用也很简单，比如你玩赛车游戏，控制左右转弯，屏幕横屏和竖屏切换，都需要用到重力感应模块。<br>
陀螺仪，又叫角速度传感器，用于测量物理量的偏转、倾斜是的动作角速度。可以精确的分析判断出使用者的实际动作，通过他收集的这些动作给手机下达一些指令。<br>
deviceorientation事件 <br>
a)要接收设备方向变化信息，你只需要注册监听deviceorientation事件 <br>
注册完事件监听处理函数后，监听函数会定期地接收到最新的设备方向数据 <br>
b)ev.absolute	如果方向数据跟地球坐标系和设备坐标系有差异，则absolute为true，如果方向数据由设备本身的坐标系提供，则absolute为false。<br>
c)ev.alpha		表示设备沿z轴上的旋转角度，范围为0~360。 <br>
d)ev.beta		表示设备在x轴上的旋转角度，范围为-180~180。它描述的是设备由前向后旋转的情况。 <br>
e)ev.gamma	表示设备在y轴上的旋转角度，范围为-90~90。它描述的是设备由左向右旋转的情况 <br>
## api文档 
https://developer.mozilla.org/zh-CN/docs/Web/API/DeviceOrientationEvent/absolute

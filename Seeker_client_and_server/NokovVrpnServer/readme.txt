V9.1更新：
可以通过输入SDK NIC Address，达到本网段或跨网段实现VRPN传输的功能
在V6.1基础上，使用回调方式获取数据，提升稳定性

V10.1更新 （Body版本/爱迪思通定制版本）
增加支持加载同目录下config.ini配置文件设定反转轴
增加支持XBOX360设备，自定义设备名称，手柄设备数据与帧数据同步（包括滑杆的坐标与按钮的状态）

测试设备：Sony Navigation Controller
蓝牙接收器为 CSR4.0 8510 芯片
要求：将PS MOVE 左手柄，虚拟成 Xbox360 手柄；
参考SONY PS move 左手柄安装说明

其中配置文件使用说明

// 追踪对象全局反转轴设定
[InvertAxisPosition] // 坐标轴
X=0
Y=0
Z=0
[InvertAxisRotation] // 旋转轴
X=0
Y=0
Z=0
// 名称Nokov的对象的特定反转设定
[Nokov] 
PX=1   // 坐标轴X
PY=1
PZ=0
RX=1 // 旋转轴X
RY=1
RZ=1
// 手柄设备
[JoyStick]
Name=PS4  //手柄名称
InvertLX=0  // 滑杆反转设定，0不反向
InvertLY=1 //  垂直反向

V11.1 更新 (通用版本) 参阅config.ini配置文件注释说明
增加支持定制转发数据类型
增加支持设定网络连接参数
增加调试打印帧率信息
采用更友好的交互方式

V12.1更新：
增加速度和加速度支持
需要配置FrameFactor（帧因子）和FrameRate（帧率）才能计算

## 关于`ONVIF-SpyDroid-Camera`

这里是将`Android`设备实现成`ONVIF`协议的`server`.

可以通过[ONVIF-Camera](https://github.com/yashrs/ONVIF-Camera.git)工程来验证`ONVIF-SpyDroid-Camera`
是否工作正常。
如果通过[ONVIF-Camera](https://github.com/yashrs/ONVIF-Camera.git)可以连接到`ONVIF-SpyDroid-Camera`
的话，就代表`Discovery`协议是可以工作。

> 目前[ONVIF-Camera](https://github.com/yashrs/ONVIF-Camera.git)有一些问题，就是拉取到`RTSP`流之后播放有问题<br>，只可以播放一帧，应该是视频格式不支持。但是通过`ffplay`是可以播放`ONVIF-SpyDroid-Camera`的`RTSP`视频流的.


--------------------------------------------------------------

ONVIF 默认地址：http://ip:8080/onvif/device_service
默认用户名：ky_lab
默认密码：123456

配置文件路径：app\src\main\java\net\majorkernelpanic\onvif\DeviceStaticInfo.java

onvif 调试：app\src\main\java\net\majorkernelpanic\onvif\SimpleONVIFManager.java 修改组播地址，
如果使用有线网络，需要将文件内wlan0修改为eth0

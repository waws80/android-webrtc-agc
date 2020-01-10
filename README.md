# android-webrtc-agc

### Android单独抽取WebRtc-AGC(语音端点检测)模块

#### csdn:https://blog.csdn.net/always_and_forever_/article/details/78472872

### 使用说明
#### 1.下载源码，直接运行即可

### 工程解读
#### 1.根目录下的jni目录，是从webrtc源码中抽取出来的agc模块核心代码文件.
#### 2.libs目录下，为编译jni生成的so文件，您可以直接使用.
#### 3.webrtc-agc.apk 可直接安装到真机上快速体验.
#### 4.test_input.pcm为测试文件，启动app将自动执行agc，agc后文件路径为手机根目录/agc_out.pcm
#### 5.如您需要体验生成so这一步骤，可cd到jni目录下，执行ndk-build命令，前提是您下载了ndk且配置了环境变量，否则ndk命令无法识别

### 测试对比
#### 1.如图中所示，上面是agc后，下面是agc前
![Image text](https://raw.githubusercontent.com/wangzhengcheng1994/android-webrtc-agc/master/pic/pic.jpg)

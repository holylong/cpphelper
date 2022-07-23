# C/C++开源库推荐
```
  主要都是平常用到的，包含windows开发、android开发、后台开发、音视频开发、深度学习等等

  最后还附带几个其他语言开发的比较好的项目
```
### GUI开发
* [qt](https://github.com/qt/qt5) 跨平台开发库，内部封装了各种跨平台工具，但是大多数情况下都被用作开发跨平台客户端
* [imgui](https://github.com/ocornut/imgui) 基于opengl/dx编写的GUI库,挺简单也挺好用的
* [electron](https://github.com/electron/electron) C++/NodeJS开发的跨平台GUI库，感觉其实就是简化版的chrome并做了某些功能的增强，分为main/render两部分，ui布局全是html/js/ts/vue/jsx，轻轻松松就可以开发出一个很漂亮的界面，毕竟前端模板太多了，可以配套用nodejs调用C++那一套，回调回C++混合开发,对执行效率要求不高的可以用
* [sdl](https://github.com/libsdl-org/SDL) 跨平台GUI开发库,scrcpy用的就是这个
* [SFML](https://github.com/SFML/SFML) 跨平台的GUI库，以前开发游戏时写了一个demo，用了一次
* [duilib](https://github.com/duilib/duilib) 美化MFC项目
* [skia](https://github.com/google/skia) google开源的gui库，android/chrome的UI都是用这个画的
* [wxwidgets](https://github.com/wxWidgets/wxWidgets) audacity好像用的就是这个gui库
* [boden](https://github.com/AshampooSystems/boden) android/ios gui库，纯C++开发
* [elements](https://github.com/cycfi/elements) 跨平台ui库

### 远程控制
* [freerdp](https://github.com/FreeRDP/FreeRDP) rdp远程控制，在windows上还是mstsc最好用，linux/mac可以考虑freerdp
* [aspia](https://github.com/aspia/aspia) p2p远程工具，研究过其中代码挺不错的
* [scrcpy](https://github.com/Genymobile/scrcpy) PC控制android手机，需要打开adb
* [synergy](https://github.com/symless/synergy-core) 效率工具，用一台机器共享鼠标键盘控制多台其他计算机，gui配置要激活，我一般直接用控制台启动，具体配置及启动方式请移步[synergy控制台启动](https://blog.csdn.net/CHNIM/article/details/125718255?csdn_share_tail=%7B%22type%22%3A%22blog%22%2C%22rType%22%3A%22article%22%2C%22rId%22%3A%22125718255%22%2C%22source%22%3A%22CHNIM%22%7D&ctrtid=9tgLN)
* [QtScrcpy](https://github.com/barry-ran/QtScrcpy) 将synergy的gui用QT重写了并做了增强
* [tigervnc](https://github.com/TigerVNC/tigervnc) 开源的vnc客户端与服务端

### 音视频开发
* [ffmpeg](https://github.com/ffmpeg/ffmpeg) 从事音视频开发必备库，avformat混流分流何种协议封装，avcodec音视频编辑器封装
* [openh264](https://github.com/cisco/openh264) 思科开源的h264编解码库，号称最快，没有具体测试过
* [x264](https://github.com/mirror/x264) h264编解码库
* [libvpx](https://github.com/webmproject/libvpx) vp8/vp9编解码库
* [vlc](https://github.com/videolan/vlc) videolan的视频播放器，可提供api接口调用很方便
* [QtAV](https://github.com/wang-bin/QtAV) 将ffmpeg封装成一个Qt播放器组件，在qt中用很方便
* [rlottie](https://github.com/Samsung/rlottie) lottie动画播放库，以前写QT项目时用到了，不过qt现在自己也有lottie播放组件了

### 音视频会议
* [webrtc](https://github.com/holylong/webrtc) google开源的为浏览器提供实时通话的C++库，在浏览器上提供了一套接口，很方便的实现p2p视频通话，最近几年因为疫情这个库被大量用于音视频会议系统
* [janus](https://github.com/meetecho/janus-gateway) 纯C开发的音视频会议服务器，很多公司的服务器都是以这个为基础版本改出来的
* [licode](https://github.com/lynckia/licode) C++/js开发的音视频会议服务器，同样被很多公司拿出来用
* [mediasoup](https://github.com/versatica/mediasoup) 基于webrtc的 sfu服务器，以库的形式开放出来，可以嵌入自己的项目中
* [media-server](https://github.com/medooze/media-server) 基于webrtc的服务器
* [freeswitch](https://github.com/signalwire/freeswitch) voip视频会议服务器
* [kamailio](https://github.com/kamailio/kamailio) sip注册服务器，编译安装配置好以后，下载个linphone就可以局域网视频通话，配置个rtpengine也可以转发rtp视频流

### 压缩库
* [p7zip](https://www.7-zip.org/) 俄罗斯同志开发的压缩解压算法库，并提供安装程序，很出名养了一大批同类软件
* [libzip](https://github.com/nih-at/libzip) 传统的zip压缩解压缩库

### 计算机视觉/深度学习
* [opencv](https://github.com/opencv/opencv) intel开源的图像处理库，里边包含了何种图像处理的算法，简单的人脸识别，抠图，图像拼接，边缘检测等等，还有dnn模块可以加载其他深度学习框架训练的模型进行推理，内部封装了ffmpeg,libjpg,libpng，支持图像io,视频io，很强大的C++计算机视觉库
* [dlib](https://github.com/davisking/dlib) 人脸检测识别库，里边包含很多功能
* [PaddlePaddle](https://github.com/PaddlePaddle/Paddle) 百度开源的深度学习框架，没有用这个训练过东西
* [pytorch](https://github.com/pytorch/pytorch) facebook开源的深度学习框架，目前学术界最流行的
* [tensorflow](https://github.com/tensorflow/tensorflow) google开源的深度学习框架
* [darknet](https://github.com/AlexeyAB/darknet) 目标检测方面的神，可惜原作者已放弃这方面的研究,现在已经有pytorch实现的yolov5,yolov7了，可以用更少的数据训练出不错的模型
* [mxnet](https://github.com/apache/incubator-mxnet) 亚马逊在用的深度学习框架
* [onnxruntime](https://github.com/microsoft/onnxruntime) 微软开源的深度学习推理框架，配合onnx使用
* [caffe](https://github.com/BVLC/caffe) 贾扬清开发的深度学习框架，以前很多人都用这个，后来tensorflow出来后，大家纷纷开始转python用tensorflow
* [mediapipe](https://github.com/google/mediapipe) google开源的推理框架，谁用谁知道，确实是快
* [ncnn](https://github.com/Tencent/ncnn) 腾讯开源的推理框架，移动端很快
* [mnn](https://github.com/alibaba/MNN) 阿里开源的推理框架
* [mace](https://github.com/XiaoMi/mace) 小米开源的模型推理框架
* [Paddle-Lite](https://github.com/PaddlePaddle/Paddle-Lite) 百度开源的推理框架
* [lite.ai.toolkit](https://github.com/DefTruth/lite.ai.toolkit) 把一些推理框架做了封装的工具库
* [libfacedetection](https://github.com/ShiqiYu/libfacedetection) yushiqi开源的人脸检测工具
* [SeetaFace](https://github.com/seetafaceengine/SeetaFace2) 好像是中科院某位教授开源的项目，检测识别效果不错，拿来即用的项目，当时用了里边的人脸检测确实是最快的

### 语音识别/深度学习
* [kaldi](https://github.com/kaldi-asr/kaldi) 语音识别方面必知必会的库，以前研究过一段时间，程序不怎么用修改，需要修改shell脚本，而且训练的比较慢，我所属的公司都是快节奏的公司，后来就直接改用其他公司产品了，就再没有研究过
* [wenet](https://github.com/wenet-e2e/wenet) 国内某公司开源的语音识别系统，使用pytorch推理，效果比自己训练的kaidi好
* [PaddleSpeech](https://github.com/PaddlePaddle/PaddleSpeech) 百度开源的语音识别项目，效果比wenet好
* [DeepSpeech](https://github.com/mozilla/DeepSpeech) 语音识别项目
* [audacity](https://github.com/audacity/audacity) 语料分析调整工具
* [portaudio](https://github.com/PortAudio/portaudio) audioio工具

### 服务器
* [nginx](https://github.com/nginx/nginx) 俄罗斯同志开发的http服务器，代理服务器，还支持各种协议，用过的都说好，不过现在属于美国公司了
* [srs](https://github.com/ossrs/srs) 以前用他当做rtmp服务器
* [ZLMediaKit](https://github.com/ZLMediaKit/ZLMediaKit) 媒体服务器
* [redis](https://github.com/redis/redis) 缓存服务器，用来存储临时变量很方便，与db协同使用
* [httpd](https://github.com/apache/httpd) apache开源的web服务器
* [lighttpd](https://github.com/lighttpd/lighttpd1.4) 轻量级的web服务器
* [memcached](https://github.com/memcached/memcached) 缓存服务器，类似于redis
* [kbengine](https://github.com/kbengine/kbengine) C++开发的游戏服务器

### 游戏
* [cocos2d-x](https://github.com/cocos2d/cocos2d-x) cocos2d-x是一个C++开发的跨平台游戏开发库，现在游戏开发用cocos的应该比较少，大部分都是unity/ue4
* [UnrealEngine](https://github.com/EpicGames/UnrealEngine) 渲染效果最好的游戏引擎

### 序列化
* [protobuf](https://github.com/protocolbuffers/protobuf) 很常用的序列化工具，具有比json占用空间小，编解速度快的特点
* [json](https://github.com/nlohmann/json) modern c++开发的json解析库
* [jsoncpp](https://github.com/open-source-parsers/jsoncpp) c++开发的json解析库
* [tinyxml2](https://github.com/leethomason/tinyxml2) C++开发的xml解析库
* [rapidjson](https://github.com/Tencent/rapidjson) 腾讯开源的json解析库
* [pugixml](https://github.com/zeux/pugixml) 支持xpath的xml解析库

### 网络库
* [libevent](https://github.com/libevent/libevent) event驱动的跨平台网络库
* [libuv](https://github.com/libuv/libuv) 专门为nodejs开发的event库，是个独立的项目可以单独拿来用
* [wangle](https://github.com/facebook/wangle) facebook开源的网络库，根据java netty架构设计的，习惯netty的可以试试
* [muduo](https://github.com/chenshuo/muduo) reactor模式网络库
* [grpc](https://github.com/grpc/grpc) google开源的rpc项目
* [brpc](https://github.com/apache/incubator-brpc) 百度开源的rpc项目，捐给了apache基金会，据说很强
* [asio](https://github.com/chriskohlhoff/asio) modern C++实现的网络库
* [thrift](https://github.com/apache/thrift) apache基金会旗下的rpc项目
* [rpclib](https://github.com/rpclib/rpclib) 以前想找个小的rpc项目研究，就研究的这个
* [crow](https://github.com/ipkn/crow) modern c++ web服务器，类似于flask
* [curl](https://github.com/curl/curl) http客户端项目
* [librdkafka](https://github.com/edenhill/librdkafka) 读写kafka服务器的client,以前搞大数据是用过
* [zmq](https://github.com/zeromq/libzmq) 与其他mq项目不同，zmq是以库的形式提供

### 数据库
* [postgresql](https://github.com/postgres/postgres) 很流行的sql服务器
* [mysql](https://github.com/mysql/mysql-server) 项目中用的最多的sql服务器
* [mongodb](https://github.com/mongodb/mongo) 是一个基于分布式文件存储的数据库。由C++语言编写。旨在为WEB应用提供可扩展的高性能数据存储解决方案。
* [sqlite](https://github.com/sqlite/sqlite) 一款轻型的数据库，一般嵌入到项目内部
* [leveldb](https://github.com/google/leveldb) google开源的非常高效的kv数据库
* [mmkv](https://github.com/Tencent/MMKV) 腾讯开源的高效kv数据库

### 加密解密
* [openssl](https://github.com/openssl/openssl) 加密解密库
* [boringssl](https://github.com/google/boringssl) google从openssl中分离出来的加密解密库
* [mbedtls](https://github.com/Mbed-TLS/mbedtls) 嵌入式项目中经常用的加密解密库

### 虚拟机
* [qemu](https://github.com/qemu/qemu) ffmpeg作者开源的模拟器，据说可以达到真机效果
* [virtualbox](https://www.virtualbox.org/) oracle开源的x86模拟器
* [botchs](https://sourceforge.net/projects/bochs/) x86模拟器
* [anbox](https://github.com/anbox/anbox) 感觉像是一个把android虚拟机跑在linux上的东西，android上的每个程序直接绘制在linux gui上

### 编译器
* [gcc](https://github.com/gcc-mirror/gcc) gcc编译器
* [llvm](https://github.com/llvm/llvm-project) llvm编译套件

### 工具库
* [folly](https://github.com/facebook/folly) facebook开源的基础库
* [abseil-cpp](https://github.com/abseil/abseil-cpp) google开源的基础库
* [boost](https://github.com/boostorg/boost) boost工具库
* [concurrentqueue](https://github.com/cameron314/concurrentqueue) 并发队列

### 构建工具
* [cmake](https://github.com/Kitware/CMake) 跨平台构建工具，用的最广泛的工具，android/linux/windows几乎哪都再用
* [ninja](https://github.com/ninja-build/ninja) google工程师开源的构建工具类似于make
* [vcpkg](https://github.com/microsoft/vcpkg) 相当于ubuntu上的apt-get install吧,只不过，vcpkg是下载编译安装到仓库，并且需要配合cmake使用

### 跨平台项目
* [chromium](https://www.chromium.org/chromium-projects/) chrome浏览器开源项目，很多项目都是这个项目的子项目
* [v8](https://github.com/v8/v8) chromium项目的子项目
* [nodejs](https://github.com/nodejs/node) 基于v8开发的让js独立于浏览器运行的开发平台

### 无分类工具
* [TrafficMonitor](https://github.com/zhongyang219/TrafficMonitor) 计算机网速流量检测工具，cmake构建的版本[TrafficMonitor](https://github.com/holylong/TrafficMonitor)
* [TranslucentTB](https://github.com/TranslucentTB/TranslucentTB) 状态栏透明

## golang项目
* [frp](https://github.com/fatedier/frp) 代理工具将局域网主机暴露到公网上，远程办公必备
* [caddy](https://github.com/caddyserver/caddy) nginx的golang版本
* [docker](https://github.com/moby/moby) 轻量级虚拟机，相当于从软件层面的虚拟化，很方便
* [k8s](https://github.com/kubernetes/kubernetes) google开源的用于管理云平台中多个主机上的容器化的应用
* [minikube](https://github.com/kubernetes/minikube) k8s的单机版本
* [Open-IM-Server](https://github.com/OpenIMSDK/Open-IM-Server) 微信前团队开源的im服务器

## rust项目
* [rustdesk](https://github.com/rustdesk/rustdesk) rust开发的远程客户端，服务端不开源
* [yew](https://github.com/yewstack/yew) rust前端开发框架类似于react
* [tauri](https://github.com/tauri-apps/tauri) 类似于electron,不过速度性能都比electron强

## ts/js项目
* [simple-peer](https://github.com/feross/simple-peer) 对webrtc接口做了封装，使调用更简单了
* [deskreen](https://github.com/pavlobu/deskreen) 基于webrtc的投屏器，通过浏览器将桌面投到其他设备上

## c#项目
* [Wox](https://github.com/Wox-launcher/Wox) windows启动器

## java/kotlin项目
* [dbeaver](https://github.com/dbeaver/dbeaver) java开发的数据库连接客户端
* [libgdx](https://github.com/libgdx/libgdx) 基于java的跨平台游戏开发框架

## python项目
* [flask](https://github.com/pallets/flask) python web引擎
* [django](https://github.com/django/django) python web引擎
* [scrapy](https://github.com/scrapy/scrapy) 爬虫引擎功能很全

## dart项目
* [dio](https://github.com/flutterchina/dio) dart http网络库
* [Best-Flutter-UI-Templates](https://github.com/mitesh77/Best-Flutter-UI-Templates) flutter开发的跨平台界面，在andriod/windows跑过，ui设计的不错，就是给人一种卡顿的感觉
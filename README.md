![image](https://github.com/452693688/React-Native/blob/master/node%E4%B8%8B%E8%BD%BD1.png)
<br />
[下载页1](https://nodejs.org/)
<br />

![image](https://github.com/452693688/React-Native/blob/master/node%E4%B8%8B%E8%BD%BD2.png)
<br />
[下载页2](https://nodejs.org/dist/v6.2.0/)
<br />

参考：http://www.51itong.net/windows-react-native-19723.html
      http://www.codeceo.com/article/windows-react-native-android.html

配置SDK 环境：<br />
1.ANDROID_HOME：Android SDK Manager的位置 例如：（PATH => D:\Program Files\Android SDK Tools）<br />
2.设置环境变量PATH：例如：（PATH => %ANDROID_HOME%\tools;%ANDROID_HOME%\platform-tools）<br />
studio 2.0或者以上<br />
一：下载nodes.js<br />
  https://nodejs.org/<br />

二: 使用npm安装ReactNative
	1)npm install -g react-native-cli（注意：它是全局的）<br />
	
  2)可能遇到的问题：<br />

   报错：npm-install-save-react-native-failed<br />

   解决办法：升级nodejs及npm版本<br />

   报错：'xxx’不是内部或外部命令<br />

   解决办法：设置对应命令为环境变量或安装对应的命令工具<br />

三：构建项目<br />
	react-native init HelloAndroid（注意：它是在当前目录下创建HelloAndroid新目录）<br />
	
四：启动项目   <br />
  
 react-native start（注意：需要进入HelloAndroid项目的根目录）<br />
 
 当构建完毕，在浏览器中访问<br />
 http://localhost:8081/index.android.bundle?platform=android<br />
 可以看到我们编译好的android bundle文件。<br />

五：启动安卓项目 <br />
	react-native run-android<br />
	
六：
将js代码导成资源 目前android版本需要手动去做。<br />
参考issues。相信Facebook后面的版本会马上会发布自动导资源的命令。<br />
实际现在也挺简单：当react-native的server启动后。<br />
把http://localhost:8081/index.android.bundle?platform=android这个地址的js拷出来即可。 <br />
链接：http://www.imooc.com/article/2646<br />
 
原生安卓app转React Ntive app：<br />
http://www.lcode.org/%E3%80%90react-native%E5%BC%80%E5%8F%91%E3%80%91react-native%E7%A7%BB%E6%A4%8D%E5%8E%9F%E7%94%9Fandroid%E9%A1%B9%E7%9B%AE/<br />
七：没有node文件<br />
命令行运行npm install  --save react-native  进行安装react native模块以及相关node模块 <br />
其他：<br />
	adb reverse tcp:8081 tcp:8081<br />
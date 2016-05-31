参考：http://www.51itong.net/windows-react-native-19723.html
      http://www.codeceo.com/article/windows-react-native-android.html

配置SDK 环境：
1.ANDROID_HOME：Android SDK Manager的位置 例如：（PATH => D:\Program Files\Android SDK Tools）
2.设置环境变量PATH：例如：（PATH => %ANDROID_HOME%\tools;%ANDROID_HOME%\platform-tools）
studio 2.0或者以上
一：下载nodes.js
  https://nodejs.org/

二: 使用npm安装ReactNative
	1)npm install -g react-native-cli（注意：它是全局的）
	
  2)可能遇到的问题：

   报错：npm-install-save-react-native-failed

   解决办法：升级nodejs及npm版本

   报错：'xxx’不是内部或外部命令

   解决办法：设置对应命令为环境变量或安装对应的命令工具

三：构建项目
	react-native init HelloAndroid（注意：它是在当前目录下创建HelloAndroid新目录）
	
四：启动项目   
  
 react-native start（注意：需要进入HelloAndroid项目的根目录）
 
 当构建完毕，在浏览器中访问
 http://localhost:8081/index.android.bundle?platform=android
 可以看到我们编译好的android bundle文件。

五：启动安卓项目 
	react-native run-android
其他：
	adb reverse tcp:8081 tcp:8081
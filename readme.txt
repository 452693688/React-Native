�ο���http://www.51itong.net/windows-react-native-19723.html
      http://www.codeceo.com/article/windows-react-native-android.html

����SDK ������
1.ANDROID_HOME��Android SDK Manager��λ�� ���磺��PATH => D:\Program Files\Android SDK Tools��
2.���û�������PATH�����磺��PATH => %ANDROID_HOME%\tools;%ANDROID_HOME%\platform-tools��
studio 2.0��������
һ������nodes.js
  https://nodejs.org/

��: ʹ��npm��װReactNative
	1)npm install -g react-native-cli��ע�⣺����ȫ�ֵģ�
	
  2)�������������⣺

   ����npm-install-save-react-native-failed

   ����취������nodejs��npm�汾

   ����'xxx�������ڲ����ⲿ����

   ����취�����ö�Ӧ����Ϊ����������װ��Ӧ�������

����������Ŀ
	react-native init HelloAndroid��ע�⣺�����ڵ�ǰĿ¼�´���HelloAndroid��Ŀ¼��
	
�ģ�������Ŀ   
  
 react-native start��ע�⣺��Ҫ����HelloAndroid��Ŀ�ĸ�Ŀ¼��
 
 ��������ϣ���������з���
 http://localhost:8081/index.android.bundle?platform=android
 ���Կ������Ǳ���õ�android bundle�ļ���

�壺������׿��Ŀ 
	react-native run-android
������
	adb reverse tcp:8081 tcp:8081
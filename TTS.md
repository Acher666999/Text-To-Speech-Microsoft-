需要简单的语音识别功能，测试一下微软自带的SDK。

安装步骤：

1 安装speech sdk https://www.microsoft.com/en-us/download/details.aspx?id=27226

2 安装runtime 在speech sdk安装目录下面Microsoft SDKs\Speech\v11.0\Redist\SpeechPlatformRuntime.msi

3 安装语音包 https://download.microsoft.com/download/4/0/D/40D6347A-AFA5-417D-A9BB-173D937BEED4/MSSpeech_TTS_zh-CN_HuiHui.msi



在Windows10操作系统里，没有Yaoyao和Kangkang语音助手，需要修改注册表才能使用其他语音助手。

下面简单说明一下，如何修改注册表。打开注册表，路径如截图里所示：
计算机\HKEY_LOCAL_MACHINE\SOFTWARE\WOW6432Node\Microsoft\SPEECH\Voices\Tokens\TTS_MS_ZH-CN_HUIHUI_11.0

先导出一个Huihui注册表文件：

![1](C:\Users\Administrator\Desktop\1.png)



右键编辑：

![2](C:\Users\Administrator\Desktop\2.png)

把文件里面的“Huihui”字眼修改为“Kangkang”，约有5处需要修改。
因为Kangkang是男声，也要把"Gender"="Male"项的Female改为Male。
修改后如下图：![3](C:\Users\Administrator\Desktop\3.png)

通过这样操作，重复上面的操作，把Yaoyao注册表项也添加进去注册表。
这次只需把Huihui修改为Yaoyao。
“Gender”="Female"不用修改。

修改完成导入注册表。

![4](C:\Users\Administrator\Desktop\4.png)


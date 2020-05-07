# 安卓逆向工具汇总 / Awsome Android Reverse Tools

### 脱壳 / Unshell

* [FDex2](https://bbs.pediy.com/thread-224105.htm)
  * 安卓xposed脱壳工具
  * 通过Hook ClassLoader的loadClass方法，反射调用getDex方法取得Dex(com.android.dex.Dex类对象)，再将里面的dex写出
  * 安卓4.4以上的手机或模拟器
  * 其它看软件提示
* [FART](https://github.com/hanbinglengyue/FART)
  * ART环境下自动化脱壳方案
  * 支持6.0到8.0，理论支持任意ART系统，需要刷机
  * 更多的脱壳机镜像[AndroidSecurityStudy](https://github.com/r0ysue/AndroidSecurityStudy)


### so库 / Native

* [IDA Pro](https://www.hex-rays.com/products/ida/)
  * __目前最棒的反编译软件__（商业软件，网上可以找到破解版，真有能力的建议支持下正版）
  * 支持 java、native
  * 支持动态调试
* [Frida](https://www.frida.re/): 
  * 代码插桩工具
  * 使用Python提供API，用JavaScript编写hook代码
  * 支持hook java层
  * 支持hook native 层
* [Ghidra](https://github.com/NationalSecurityAgency/ghidra)
  * 由美国国家安全局（NSA）研究部门开发的软件逆向工程（SRE）套件
  * 支持Windows、Mac OS和Linux
  * 功能包括反汇编，汇编，反编译，绘图和脚本等
  * [[翻译]Ghidra简介](https://bbs.pediy.com/thread-250056.htm)
* [SoFixer](https://github.com/F8LEFT/SoFixer)
  * so 修复相关（支持内存 dump so 的 section 修复）
  * 原理：[[原创]简单粗暴的so加解密实现](https://bbs.pediy.com/thread-191649.htm)
  * 编译好的工具：[下载地址](https://github.com/WuFengXue/AndroidBinUtils/releases/tag/SoFixer-v0.2)

### 带界面的工具 / GUI Tools

* [jeb](https://www.pnfsoftware.com/)
  
  * 商业反编译软件(有demo版本免费)
  * 强大的将bytecode转为java代码的能力，对于循环等处理的很好
  * **支持动态编辑，重命名，添加新package等**
  * 支持python的api扩展

* [jadx-gui](https://github.com/skylot/jadx/tree/master/jadx-gui/src/main/java/jadx/gui):     

   * 方便的jadx工具，可以直接反编译apk
   * 与jd-gui有类似的界面
   * 支持全局搜索

* [GDA](https://github.com/charles2gan/GDA-android-reversing-Tool)

   * 国人开发的字节码反编译工具
   * 支持 APK、DEX、ODEX、oat

* [ClassyShark](https://github.com/google/android-classyshark)

   * Google的apk查看工具
   * 可以分析出apk的结构以及依赖信息

* [jd-gui](http://jd.benow.ca/):
  
  * 用来查看反编译.class文件
  * 支持Eclipe和IntelliJ扩展
  * 有漂亮的gui界面
  
  ![](http://java-decompiler.github.io/img/jd-gui.png)
  
* [androguard](https://github.com/androguard/androguard): 

   * 使用DAD作为反编译器
   * 可以分析恶意软件
   * 有python api，可以写扩展
   * **支持可视化**
   ![](https://raw.githubusercontent.com/Juude/droidReverse/master/art/guard.png)

* [codeinspect](http://sseblog.ec-spride.de/tools/codeinspect/)
   * 支持调试
   * 可以IDE中编辑反编译后文件
   
* [BytecodeViewer](https://bytecodeviewer.com/)   
  
  * 集成了J-RET,JHexPane, Dex2Jar等多个反编译工具

### 命令行工具 / Command Line Tools

* [apktool](https://ibotpeaches.github.io/Apktool/): 
  * 编译res资源
  * 转成smali
  * 将修改后的smali回编译为apk

* [enjarfy](https://github.com/google/enjarify)：
  * google的反编译工具
  * 可以将dalvik bytecode转化为java bytecode
  * 比dex2jar支持case更多

* [dex2jar](https://github.com/pxb1988/dex2jar): 
  * dex转为jar工具
  * 转成smali并且回编译

* [smali/baksmali/smalidea](https://github.com/JesusFreke/smali)
  * 将dex反编译成smali
  * 将smali回编译成dex
  * AndroidStudio调试smali代码

* [icodetools](https://github.com/fourbrother/icodetools)
  * 动态插入log代码到apk中的每个方法中的工具
  * 只支持JDK1.7以及以下版本编译器
* [AXmlPrinter2](http://code.google.com/p/android4me/downloads/list)
  * 反编译Androidmanifest.xml的工具
  * 反编译后的结果会输出到控制台
  * 当前已经很少使用了

### 抓包 / Web Debugging Proxy

* [Charles](https://www.charlesproxy.com/)
  * 网络抓包工具

### 插件 / Plugin

* [java2smali](https://github.com/ollide/intellij-java2smali)
  * Android Studio插件
  * 支持将java和Kotlin文件编译成smali文件

### 游戏 / Games

* [ILSpy](https://github.com/icsharpcode/ILSpy)
  * 开源的 .NET 反编译工具
* [dnSpy](https://github.com/0xd4d/dnSpy)
  * 开源的 .NET 调试和反编译工具
* [.NET Reflector](http://www.red-gate.com/products/dotnet-development/reflector/)
  * dll反编译工具
* [UnityStudio](https://github.com/Perfare/UnityStudio)
  * Unity游戏资源提取工具
  * 支持资源预览
* [Il2CppDumper](https://github.com/Perfare/Il2CppDumper)
  * Windows 平台下的 Unity il2cpp 逆向工具
  * 还原DLL文件（不包含代码），可用于提取`MonoBehaviour`和`MonoScript`
  * 生成IDA和Ghidra的脚本，帮助IDA和Ghidra更好的分析il2cpp文件
* [GameGuardian](https://gameguardian.net/download)
  * a game cheat / hack / alteration tool
  * modify money, HP, SP, and much more
  * **ROOT or VIRTUAL ENVIRONMENT ONLY**
* [get_dll_from_bin.exe](https://gameguardian.net/forum/files/file/7-utility-for-extracting-dll-files-from-various-dumps/)
  * extracts PE-files (.exe, .dll, etc.) from .bin files.
  * [How to dump DLL and other files using GameGuardian (root only) (Android 2.3.3-8.0) - iAndroHacker.net](https://gameguardian.net/forum/topic/17965-how-to-dump-dll-and-other-files-using-gameguardian-root-only-android-233-80-iandrohackernet/)



## [**工具下载**](https://pan.baidu.com/s/1wLQyg6JD8MnJgklhlfczZw)   **提取码**: 3afd



## [附：逆向博文汇总](https://github.com/WuFengXue/android-reverse/blob/master/post.md)
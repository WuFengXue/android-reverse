# android-reverse

### 安卓逆向工具汇总

* [FDex2](https://bbs.pediy.com/thread-224105.htm)
  * 安卓xposed脱壳工具
  * 通过Hook ClassLoader的loadClass方法，反射调用getDex方法取得Dex(com.android.dex.Dex类对象)，再将里面的dex写出
  * 安卓4.4以上的手机或模拟器
  * 其它看软件提示

+ [Frida](https://www.frida.re/): 

  + 代码插桩工具
  + 使用Python提供API，用JavaScript编写hook代码
  + 支持hook java层
  + 支持hook native 层
+ [apktool](https://ibotpeaches.github.io/Apktool/): 

  + 编译res资源
  + 转成smali
  + 将修改后的smali回编译为apk
+ [dex2jar](https://github.com/pxb1988/dex2jar): 

  + dex转为jar工具
  + 转成smali并且回编译
+ [jd-gui](http://jd.benow.ca/):
  + 用来查看反编译.class文件
  + 支持Eclipe和IntelliJ扩展
  + 有漂亮的gui界面
  
    ![](http://jd.benow.ca/img/screenshot17.png)

+ [jadx-gui](https://github.com/skylot/jadx/tree/master/jadx-gui/src/main/java/jadx/gui):     

    + 方便的jadx工具，可以直接反编译apk
    + 与jd-gui有类似的界面
![](https://camo.githubusercontent.com/bd3c0ea851c23c4535e43590a86c940a0786faa6/687474703a2f2f736b796c6f742e6769746875622e696f2f6a6164782f6a6164782d6775692e706e67)
+ [androguard](https://github.com/androguard/androguard): 

   + 使用DAD作为反编译器
   + 可以分析恶意软件
   + 有python api，可以写扩展
   + **支持可视化**
![](https://raw.githubusercontent.com/Juude/droidReverse/master/art/guard.png)
+ [enjarfy](https://github.com/google/enjarify)：
   + google的反编译工具
   + 可以将dalvik bytecode转化为java bytecode
   + 比dex2jar支持case更多
+ [jeb](https://www.pnfsoftware.com/)
   + 商业反编译软件(有demo版本免费)
   + 强大的将bytecode转为java代码的能力，对于循环等处理的很好
   + **支持动态编辑，重命名，添加新package等**
   + 支持python的api扩展
+ [codeinspect](http://sseblog.ec-spride.de/tools/codeinspect/)
   + 支持调试
   + 可以IDE中编辑反编译后文件
+ [BytecodeViewer](https://bytecodeviewer.com/)   
  
  + 集成了J-RET,JHexPane, Dex2Jar等多个反编译工具
+ [ClassyShark](https://github.com/google/android-classyshark)
   + Google的apk查看工具
   + 可以分析出apk的结构以及依赖信息
+ [smali/baksmali/smalidea](https://github.com/JesusFreke/smali)
  + 将dex反编译成smali
  + 将smali回编译成dex
  + AndroidStudio调试smali代码
+ [AXmlPrinter2](http://code.google.com/p/android4me/downloads/list)
  + 反编译Androidmanifest.xml的工具
  + 反编译后的结果会输出到控制台
  + 当前已经很少使用了
+ [Charles](https://www.charlesproxy.com/)
  
  + 网络抓包工具
+ [.NET Reflector](http://www.red-gate.com/products/dotnet-development/reflector/)
  
  + dll反编译工具
+ [UnityStudio](https://github.com/Perfare/UnityStudio)
  + Unity游戏资源提取工具
  + 支持资源预览
+ [icodetools](https://github.com/fourbrother/icodetools)
  + 动态插入log代码到apk中的每个方法中的工具
  + 只支持JDK1.7以及以下版本编译器
+ [java2smali](https://github.com/ollide/intellij-java2smali)
  + Android Studio插件
  + 支持将java和Kotlin文件编译成smali文件

[**工具下载**](https://pan.baidu.com/s/1wLQyg6JD8MnJgklhlfczZw)   **提取码**: 3afd

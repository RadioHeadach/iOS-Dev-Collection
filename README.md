# iOS-Dev-Collection

这里主要存放我收集的 iOS 开发相关的资料和笔记，我会按照内容对应的 iOS 开发知识点来分类。

## 目录

   * [iOS-Dev-Collection](#ios-dev-collection)
      * [Objc](#objc)
         * [运行时](#运行时)
            * [non fragile ivars](#non-fragile-ivars)
      * [网络](#网络)
         * [Socket](#socket)
      * [推送](#推送)
         * [推送扩展](#推送扩展)

---

## Objc

### 语言相关
- [把OC代码 编译成C/C++](https://www.jianshu.com/p/71bdafff72ac) —— OC 转 C++ 的命令

### 运行时

- [理解 Objective-C 运行时](https://juejin.im/post/5a951ceb5188257a8929dbc1#heading-7) —— 详细描述 objc 的运行时机制的实现 

#### non fragile ivars

- [objective-c non-fragile ivars 学习笔记](https://blog.csdn.net/fly1183989782/article/details/81050782) —— 简单讲解 non-fragile ivars 的原理和为什么 category 不能添加成员变量

- [Objective-C 动态之 Non-fragile ivar](http://jefferyfan.com/programing/iOS/non-fragile-ivar/) —— 详细讲解 non-fragile ivars 的实现

- [WWDC2016 Optimizing App Startup Time](https://developer.apple.com/videos/play/wwdc2016/406/) —— WWDC 2016 关于应用启动优化的 Keynote ，里面也有提到 non-fragile ivars

## 网络

### Socket

- [局域网内通过Socket传输文件(Android&iOS可传输)](https://www.jianshu.com/p/8738d32e5668)  —— 目前认为很优秀的局域网内 Socket 传输文件的案例

## 推送

### 推送扩展

> 这里的推送扩展主要指的是之前工作中使用到的 `UNNotificationServiceExtension` ，推送通知扩展

- [iOS12中推送通知新特性-分组](https://www.jianshu.com/p/4961b425213a) —— iOS 12 之后可以通过 UNNotificationServiceExtension 对推送进行分组

- [ios UNNotificationServiceExtension app和extension的通信](https://www.jianshu.com/p/26b96b991eaf) —— 详细讲解了怎么使用和调试 UNNotificationServiceExtension

- [iOS使用Notification Service Extension统计iOS 10后的Push到达率](https://www.jianshu.com/p/ef65afc95c4a) —— 这篇文章也讲解了怎么使用 UNNotificationServiceExtension

## UIKit

### WKWebView
- [[<WKContentView 0x7ff4f2068a00> valueForUndefinedKey:]: this class is not key value coding-compliant for the key webSelectionAssistant](https://stackoverflow.com/questions/55413844/wkcontentview-not-key-value-coding-compliant-for-key-webselectionassistant) —— 我在模拟器调试网页的时候，修改页面文字内容就会报错，原因是打开了全局断点。

### Transform
- [iOS：重识Transform和frame](https://www.jianshu.com/p/e1fec2f92c63) -- 让我理解了 transform 对 frame 的影响，重新认识了 frame。

## AVFoundation

### AVPlayerLayer
= [iOS 基于AVPlayer封装的播放器，全屏切换，切换播放源](https://www.jianshu.com/p/84abeb68fb62) -- 其实对 PlayerLayer 的旋转操作就是对 layer 的旋转操作，我对 layer 还不够熟悉。
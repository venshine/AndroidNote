Android 进阶笔记
==

[English](README.md) | 简体中文

精选 Android 开发相关的官方文档、开源框架、博客社区与经典书籍。

> 最后更新：2026-10-30。收录的链接均在更新时验证可访问；已停止维护、已归档或无法访问的内容已移除。

大纲
--
> * [技术框架](#第一部分技术框架)
>   * [官方指南与示例](#官方指南与示例)
>   * [Kotlin 与协程](#kotlin-与协程)
>   * [Jetpack Compose 与 UI](#jetpack-compose-与-ui)
>   * [跨平台](#跨平台)
>   * [Jetpack 架构组件](#jetpack-架构组件)
>   * [图片加载](#图片加载)
>   * [网络请求](#网络请求)
>   * [数据库](#数据库)
>   * [JSON 解析](#json-解析)
>   * [依赖注入](#依赖注入)
>   * [响应式编程](#响应式编程)
>   * [端侧 AI 与大模型](#端侧-ai-与大模型)
>   * [构建与性能](#构建与性能)
>   * [稳定性监控](#稳定性监控)
>   * [测试](#测试)
>   * [图表](#图表)
>   * [日志框架](#日志框架)
>   * [动态化与热修复](#动态化与热修复)
>   * [新平台与新能力](#新平台与新能力)
> * [博客社区](#第二部分博客社区)
>   * [个人博客](#个人博客)
>   * [团队博客](#团队博客)
>   * [技术社区](#技术社区)
>   * [技术周报](#技术周报)
> * [技术书籍](#第三部分技术书籍)
>   * [计算机基础](#计算机基础)
>   * [操作系统](#操作系统)
>   * [体系结构](#体系结构)
>   * [计算机网络](#计算机网络)
>   * [数据库](#数据库-1)
>   * [编译原理](#编译原理)
>   * [数据结构&算法](#数据结构算法)
>   * [设计模式](#设计模式)
>   * [软件工程](#软件工程)
>   * [数字图像处理](#数字图像处理)
>   * [计算机图形学](#计算机图形学)
>   * [Linux](#linux)
>   * [Android](#android)


第一部分&nbsp;&nbsp;&nbsp;&nbsp;技术框架
--
### 官方指南与示例
* [Android 应用架构指南](https://developer.android.com/topic/architecture) -- 官方推荐的分层架构与最佳实践
* [Now in Android](https://github.com/android/nowinandroid) -- 官方完整示例应用，全面采用 Kotlin、Compose 与现代架构
* [architecture-samples](https://github.com/android/architecture-samples) -- 官方架构示例
* [compose-samples](https://github.com/android/compose-samples) -- 官方 Compose 示例集
* [Android 官方课程](https://developer.android.com/courses)
* [Android 版本与行为变更](https://developer.android.com/about/versions) -- 各版本新特性与适配要求

### Kotlin 与协程
* [Kotlin 官方文档](https://kotlinlang.org/docs/home.html)
* [Android 上的 Kotlin](https://developer.android.com/kotlin)
* [Kotlin 协程](https://developer.android.com/kotlin/coroutines) -- 官方异步编程方案，源码见 [kotlinx.coroutines](https://github.com/Kotlin/kotlinx.coroutines)
* [Kotlin Flow](https://developer.android.com/kotlin/flow) -- 异步数据流，也可替代 EventBus 等事件总线
* [kotlinx-datetime](https://github.com/Kotlin/kotlinx-datetime) -- 多平台日期时间库

### Jetpack Compose 与 UI
* [Jetpack Compose](https://developer.android.com/compose) -- 官方声明式 UI 框架
* [Material Design 3](https://m3.material.io/) -- 设计规范，Compose 实现见 [Material 3 in Compose](https://developer.android.com/develop/ui/compose/designsystems/material3)
* [Navigation 3](https://developer.android.com/guide/navigation/navigation-3) -- 面向 Compose 的新一代导航库
* [Edge-to-edge 全面屏适配](https://developer.android.com/develop/ui/views/layout/edge-to-edge)
* [View Binding](https://developer.android.com/topic/libraries/view-binding) -- 替代已停止维护的 Butter Knife
* [Circuit](https://github.com/slackhq/circuit) -- Slack 开源的 Compose 驱动架构
* [Lottie](https://lottie.airbnb.tech/) -- Airbnb 开源的动画库

### 跨平台
* [Kotlin Multiplatform](https://kotlinlang.org/docs/multiplatform.html) -- 在 Android、iOS、桌面与 Web 间共享 Kotlin 代码
* [Android 官方 KMP 指南](https://developer.android.com/kotlin/multiplatform)
* [Compose Multiplatform](https://kotlinlang.org/compose-multiplatform/) -- JetBrains 的跨平台 Compose UI，源码见 [compose-multiplatform](https://github.com/JetBrains/compose-multiplatform)

### Jetpack 架构组件
* [Room](https://developer.android.com/training/data-storage/room) -- 官方 SQLite ORM
* [DataStore](https://developer.android.com/topic/libraries/architecture/datastore) -- 替代 SharedPreferences
* [WorkManager](https://developer.android.com/develop/background-work/background-tasks/persistent) -- 可靠的后台任务调度
* [Paging 3](https://developer.android.com/topic/libraries/architecture/paging/v3-overview) -- 分页加载

### 图片加载
* [Coil](https://coil-kt.github.io/coil/) -- Kotlin 优先，支持 Compose 与 Kotlin Multiplatform
* [Glide](https://github.com/bumptech/glide)
* [Fresco](https://frescolib.org/) -- 仓库已迁移至 [meta/fresco](https://github.com/meta/fresco)

### 网络请求
* [OkHttp](https://lysine.dev/okhttp/) -- 仓库已迁移至 [lysine-dev/okhttp](https://github.com/lysine-dev/okhttp)
* [Retrofit](https://lysine.dev/retrofit/) -- 仓库已迁移至 [lysine-dev/retrofit](https://github.com/lysine-dev/retrofit)
* [Ktor](https://ktor.io/) -- JetBrains 的 Kotlin 多平台网络框架
* [Wire](https://github.com/square/wire) -- gRPC 与 Protocol Buffers

### 数据库
* [Room](https://developer.android.com/training/data-storage/room)
* [SQLDelight](https://sqldelight.github.io/sqldelight/) -- 由 SQL 生成类型安全的 Kotlin API，支持多平台
* [ObjectBox](https://github.com/objectbox/objectbox-java) -- 对象数据库，支持端侧向量检索

### JSON 解析
* [kotlinx.serialization](https://kotlinlang.org/docs/serialization.html) -- Kotlin 官方序列化库
* [Moshi](https://github.com/square/moshi)
* [Gson](https://github.com/google/gson)
* [Jackson](https://github.com/FasterXML/jackson)
* [fastjson2](https://github.com/alibaba/fastjson2) -- 替代已归档的 fastjson

### 依赖注入
* [Hilt](https://developer.android.com/training/dependency-injection/hilt-android) -- 官方推荐，基于 Dagger
* [Dagger](https://dagger.dev/)
* [Koin](https://insert-koin.io/) -- 轻量的 Kotlin 依赖注入框架
* [Metro](https://github.com/ZacSweers/metro) -- 编译期、多平台的 Kotlin 依赖注入框架
* [kotlin-inject](https://github.com/evant/kotlin-inject)

### 响应式编程
* [Kotlin Flow](https://developer.android.com/kotlin/flow)
* [RxJava](https://github.com/ReactiveX/RxJava)
* [RxAndroid](https://github.com/ReactiveX/RxAndroid)

### 端侧 AI 与大模型
* [Android AI 开发指南](https://developer.android.com/ai)
* [Gemini Nano](https://developer.android.com/ai/gemini-nano) -- 运行在设备上的 Gemini 模型
* [ML Kit GenAI API](https://developers.google.com/ml-kit/genai) -- 基于端侧模型的摘要、改写、图片描述等能力
* [Firebase AI Logic](https://firebase.google.com/docs/ai-logic) -- 在 App 中直接调用云端 Gemini 模型
* [LiteRT](https://developers.google.com/edge/litert) -- TensorFlow Lite 的继任者，端侧机器学习与生成式 AI 运行时
* [MediaPipe](https://developers.google.com/edge/mediapipe/solutions/guide) -- 端侧机器学习解决方案
* [Koog](https://github.com/JetBrains/koog) -- JetBrains 开源的 Kotlin AI Agent 框架
* [ai-samples](https://github.com/android/ai-samples) -- 官方 AI 示例
* [Gemini in Android Studio](https://developer.android.com/studio/gemini/overview) -- Android Studio 内置的 AI 编程助手

### 构建与性能
* [KSP](https://github.com/google/ksp) -- Kotlin 符号处理，替代 kapt，迁移见 [官方指南](https://developer.android.com/build/migrate-to-ksp)
* [版本目录](https://developer.android.com/build/migrate-to-catalogs) -- 统一管理依赖版本
* [R8 应用优化](https://developer.android.com/topic/performance/app-optimization/enable-app-optimization) -- 代码压缩、混淆与优化
* [Baseline Profiles](https://developer.android.com/topic/performance/baselineprofiles/overview) -- 提升启动与运行性能
* [Macrobenchmark](https://developer.android.com/topic/performance/benchmarking/macrobenchmark-overview) -- 启动、滑动等场景的性能基准测试
* [Perfetto](https://perfetto.dev/) -- 系统级性能追踪与分析
* [LeakCanary](https://square.github.io/leakcanary/) -- 内存泄漏检测
* [KOOM](https://github.com/KwaiAppTeam/KOOM) -- 快手开源的 OOM 监控
* [16 KB 页面大小适配](https://developer.android.com/guide/practices/page-sizes)

### 稳定性监控
* [Firebase Crashlytics](https://firebase.google.com/docs/crashlytics)
* [Sentry](https://github.com/getsentry/sentry-java)
* [ACRA](https://github.com/ACRA/acra)

### 测试
* [Android 测试指南](https://developer.android.com/training/testing)
* [Compose 测试](https://developer.android.com/develop/ui/compose/testing)
* [Robolectric](https://github.com/robolectric/robolectric) -- 在 JVM 上运行 Android 测试
* [MockK](https://github.com/mockk/mockk) -- Kotlin Mock 框架
* [Turbine](https://github.com/cashapp/turbine) -- Kotlin Flow 测试库
* [Paparazzi](https://github.com/cashapp/paparazzi) -- 无需设备的截图测试
* [Roborazzi](https://github.com/takahirom/roborazzi) -- 基于 Robolectric 的截图测试

### 图表
* [Vico](https://github.com/patrykandpatrick/vico) -- 支持 Compose Multiplatform 的图表库
* [MPAndroidChart](https://github.com/PhilJay/MPAndroidChart)

### 日志框架
* [Timber](https://github.com/JakeWharton/timber)
* [Logger](https://github.com/orhanobut/logger)

### 动态化与热修复
* [Tinker](https://github.com/Tencent/tinker) -- 腾讯开源的热修复方案
* [Shadow](https://github.com/Tencent/Shadow) -- 腾讯开源的零反射全动态插件框架

### 新平台与新能力
* [Android XR](https://developer.android.com/develop/xr)
* [Credential Manager](https://developer.android.com/identity/credential-manager) -- 统一的通行密钥、密码与联合登录 API

第二部分&nbsp;&nbsp;&nbsp;&nbsp;博客社区
--
### 个人博客
* [老罗的Android之旅](https://blog.csdn.net/luoshengyang)
* [Trinea](https://www.trinea.cn/)
* [郭霖](https://blog.csdn.net/guolin_blog)
* [夏安明](https://blog.csdn.net/xiaanming)
* [鸿洋](https://blog.csdn.net/lmj623565791)
* [任玉刚](https://blog.csdn.net/singwhatiwanna)
* [stormzhang](https://stormzhang.com/)
* [马天宇](https://github.com/litesuits)
* [阮一峰的网络日志](https://www.ruanyifeng.com/blog/)
* [张涛-开源实验室](http://blog.kymjs.com/)
* [谢权SELF](https://xiequan.info/)
* [何红辉（Mr.Simple）](https://blog.csdn.net/bboyfeiyu)
* [技术小黑屋](https://droidyue.com/)
* [eclipse_xu](https://blog.csdn.net/eclipsexys)
* [子墨博客](https://blog.csdn.net/ElinaVampire)
* [巫山老妖](https://blog.csdn.net/wwj_748)
* [AigeStudio](https://blog.csdn.net/aigestudio)
* [雨松MOMO程序研究院](https://www.xuanyusong.com/)
* [包建强](https://blog.csdn.net/jspandasp)
* [邓凡平](https://blog.csdn.net/innost)
* [Piasy](https://blog.piasy.com/)
* [元斌](https://blog.csdn.net/qibin0506)
* [赵四](https://blog.csdn.net/jiangwei0910410003)
* [weishu](https://weishu.me/)
* [严振杰](https://blog.csdn.net/yanzhenjie1003)
* [猴子搬来的救兵](https://blog.csdn.net/mynameishuangshuai)
* [markzhai](http://blog.zhaiyifan.cn/)
* [兰亭风雨](https://blog.csdn.net/ns_code)
* [谦虚的天下](https://www.cnblogs.com/qianxudetianxia)
* [工匠若水](https://blog.csdn.net/yanbober)
* [diygreen](https://www.jianshu.com/u/0ad0a0afc409)
* [左飞](https://blog.csdn.net/baimafujinji)
* [Frodo](http://frodoking.github.io/)
* [拉丁吴](https://www.jianshu.com/u/1d8042233f67)
* [Carson_Ho](https://blog.csdn.net/carson_ho)
* [Gityuan](http://gityuan.com/)
* [GcsSloop](https://www.gcssloop.com/)
* [frank的专栏](https://blog.csdn.net/briblue)
* [Gavin Liu](https://www.gavinliu.cn/)
* [SpikeKing](https://www.jianshu.com/u/e2b4dd6d3eb4)
* [田野光的技术小站](https://wangyeming.github.io/)
* [Coder-Pig](https://blog.csdn.net/coder_pig)
* [Android Performance](https://www.androidperformance.com/)
* [欧阳鹏](https://blog.csdn.net/ouyang_peng)
* [寒江蓑笠](https://www.heqiangfly.com/)
* [却把清梅嗅](https://juejin.cn/user/1503787635450584)
* [bugstack虫洞栈](https://bugstack.cn/)
* [奋飞安全](http://91fans.com.cn/)

### 团队博客
* [Android Developers Blog](https://android-developers.googleblog.com/) -- Android 官方技术博客
* [Kotlin Blog](https://blog.jetbrains.com/kotlin/) -- Kotlin 官方博客
* [美团技术团队](https://tech.meituan.com/)
* [腾讯 AlloyTeam](http://www.alloyteam.com/)
* [Square Developer Blog](https://developer.squareup.com/blog/)
* [Meta Engineering](https://engineering.fb.com/)
* [腾讯游戏安全实验室](https://gslab.qq.com/)

### 技术社区
* [CSDN](https://www.csdn.net/)
* [博客园](https://www.cnblogs.com/)
* [51CTO](http://www.51cto.com/)
* [开源中国](https://www.oschina.net/)
* [CocoaChina](http://www.cocoachina.com/)
* [深度开源](https://www.open-open.com/)
* [稀土掘金](https://juejin.cn/)
* [IBM Developer](https://developer.ibm.com/)
* [SegmentFault](https://segmentfault.com/)
* [InfoQ](https://www.infoq.cn/)
* [ChinaUnix](https://blog.chinaunix.net/)
* [ITPUB](https://blog.itpub.net/)
* [开发者头条](https://toutiao.io/)
* [菜鸟教程](https://www.runoob.com/)
* [V2EX](https://www.v2ex.com/)
* [FreeBuf](https://www.freebuf.com/)
* [Google开发者官方频道](http://i.youku.com/i/UMjczOTc0NDkzNg==)
* [GDG中国社区论坛](https://www.chinagdg.com/)
* [小专栏](https://xiaozhuanlan.com/)

### 技术周报
* [Android Weekly](https://androidweekly.net/)
* [Kotlin Weekly](https://kotlinweekly.net/)
* [Android开发技术周报](https://androidweekly.io/)
* [平安金融科技移动技术周报](https://www.jianshu.com/notebooks/2983917/latest)

第三部分&nbsp;&nbsp;&nbsp;&nbsp;技术书籍
--

### 计算机基础
* [《计算机科学导论》](https://book.douban.com/subject/1142213/)  
本书是大学计算机相关专业的基础课教材，涉及到计算机科学的各个方面。本书着重讲解基本概念而不是数学模型和技术细节，通过大量的图表和演示范例讲解计算机科学的基础知识。

* [《深入理解计算机系统（第3版）》](https://book.douban.com/subject/26912767/)  
本书从程序员的视角详细阐述计算机系统的本质概念，并展示这些概念如何实实在在地影响应用程序的正确性、性能和实用性。第 3 版全面基于 x86-64 体系结构。

### 操作系统
* [《现代操作系统（原书第4版）》](https://book.douban.com/subject/27096665/)  
本书是操作系统领域的经典之作，书中集中讨论了操作系统的基本原理，包括进程、线程、存储管理、文件系统、输入/输出、死锁等，同时还包含了有关计算机安全、多媒体操作系统、掌上计算机操作系统、微内核、多核处理机上的虚拟机以及操作系统设计等方面的内容。

* [《操作系统：精髓与设计原理（第8版）》](https://book.douban.com/subject/30770794/)  
本书不仅全面地讲述了操作系统的基本概念、原理和方法，还清楚地展现了当代操作系统的本质和特点。作者针对近几年操作系统领域的最新变化，对操作系统的设计原理进行深入的阐述，同时将其对操作系统整个领域全面而深入的理解呈现给读者。

### 体系结构
* [《计算机体系结构：量化研究方法（第6版）》](https://book.douban.com/subject/36108789/)  
本书是最权威的计算机体系结构著作，是久负盛名的经典作品。书中系统地介绍了计算机系统的设计基础、指令集系统结构、流水线和指令集并行技术、层次化存储系统与存储设备、互连网络以及多处理器系统等重要内容。

* [《计算机组成与设计：硬件/软件接口（原书第5版）》](https://book.douban.com/subject/26604008/)  
本书是计算机组成的经典教材。全书着眼于当前计算机设计中最基本的概念，展示了软硬件间的关系，并全面介绍当代计算机系统发展的主流技术和最新成就。

* [《计算机组成与体系结构：性能设计》](https://book.douban.com/subject/6398113/)  
本书是介绍当代计算机体系主流技术和最新技术的优秀教材，以Intel x86和ARM两个处理器系列为例，深入讨论了计算机组成与体系结构的基本原理和概念，并将它们运用到当代计算机系统设计的问题中。

* [《计算机组成与体系结构》](https://book.douban.com/subject/1881545/)  
本书系统介绍计算机组成与体系结构，主要内容包括：数字逻辑和数字系统、机器层次的数据表示方法、汇编层次的机器组织和结构、存储器的组成和结构、接口和通信、功能组织、多处理器和可供选择的其他结构、性能增强、网络结构和分布式计算机系统等。

* [《计算机组织与体系结构》](https://book.douban.com/subject/1737686/)  
本书是介绍当代计算机体系主流技术的最新技术的优秀教材。作者以Intel Pentium 4和IBM/Motorola PowerPC作为考察实例，将当代计算机系统性能问题和计算机组织与体系结构的基本概念及原理紧密联系起来。

### 计算机网络
* [《计算机网络》](https://book.douban.com/subject/10510747/)  
本书是国内外使用最广泛、最权威的计算机网络经典教材。全书按照网络协议模型自下而上（物理层、数据链路层、介质访问控制层、网络层、传输层和应用层）有系统地介绍了计算机网络的基本原理，并结合Internet给出了大量的协议实例。在讲述网络各层次内容的同时，还与时俱进地引入了最新的网络技术，包括无线网络、3G蜂窝网络、RFID与传感器网络、内容分发与P2P网络、流媒体传输与IP语音，以及延迟容忍网络等。

* [《计算机网络：自顶向下方法（原书第8版）》](https://book.douban.com/subject/36081529/)  
本书首创采用自顶向下的方法讲解计算机网络的原理和协议，出版以来已被几百所大学和学院选用，是业界最经典的计算机网络教材之一。

* [《深入理解计算机网络》](https://book.douban.com/subject/20560942/)  
本书结合最新计算机网络技术，全面、系统、深入地阐述了计算机网络的体系结构、工作原理，以及各种通信协议实现原理，能满足读者系统和深入地学习和研究计算机网络技术的需求。

* [《TCP/IP详解 卷1：协议（原书第2版）》](https://book.douban.com/subject/26825411/)  
一本完整而详细的 TCP/IP 协议指南，描述了属于每一层的各个协议以及它们如何在不同操作系统中运行。第 2 版由 Kevin R. Fall 更新，覆盖 IPv4 / IPv6 以及从链路层到应用层的主要协议。

* [《TCP/IP详解 卷2：实现》](https://book.douban.com/subject/1087767/)  
《TCP/IP详解·卷2：实现》完整而详细地介绍了TCP/IP协议是如何实现的。

* [《TCP/IP详解 卷3：TCP事务协议、HTTP、NNTP和UNIX域协议》](https://book.douban.com/subject/1058634/)  
《TCP/IP详解·卷3：TCP事务协议、HTTP、NNTP和UNIX域协议》是“TCP/IP详解系列”的延续。主要内容包括：TCP事务协议，即T/TCP，这是对TCP的扩展，使客户-服务器事务更快、更高效和更可靠。

* [《TCP/IP协议族》](https://book.douban.com/subject/5386194/)  
《世界著名计算机教材精选·TCP/IP协议族(第4版)》是介绍TCP/IP协议族的经典图书的最新版本。

* [《HTTP权威指南》](https://book.douban.com/subject/10746113/)  
本书详细解释了HTTP协议，包括HTTP是如何工作的，如何用HTTP来开发基于Web的应用程序，核心的因特网协议如何与架构构建块交互，如何正确实现因特网客户和服务器等。

### 数据库
* [《数据库系统概念（原书第7版）》](https://book.douban.com/subject/35501216/)  
本书是数据库领域的殿堂级作品，是夯实数据库理论基础，增强数据库技术内功的必备之选，对深入理解数据库，深入研究数据库，深入操作数据库都具有极强的指导作用。

* [《数据库系统实现》](https://book.douban.com/subject/4838430/)  
本书是关于数据库系统实现方面内容最为全面的著作之一，是美国斯坦福大学计算机科学专业数据库系列课程第二门课程的指定教材。

* [《高性能MySQL（第4版）》](https://book.douban.com/subject/36096578/)  
本书是MySQL 领域的经典之作，拥有广泛的影响力。

* [《MongoDB权威指南（第3版）》](https://book.douban.com/subject/35688800/)  
本书是一本广受好评的MongoDB权威著作。书中介绍了面向文档的存储方式及利用MongoDB的无模式数据模型处理文档、集合和多个数据库，讲述了如何执行基本的写操作以及各种复杂的条件查询，还介绍了索引、聚合工具以及其他高级查询技术，另外对监控、安全性和身份验证、备份和修复、水平扩展MongoDB数据库等内容也有所涉及。

* [《Redis设计与实现》](https://book.douban.com/subject/25900156/)  
本书系统而全面地描述了Redis内部运行机制，是NoSQL数据库开发人员案头必备。

* [《NoSQL精粹》](https://book.douban.com/subject/25662138/)  
《NoSQL精粹》为考虑是否可以使用和如何使用NoSQL数据库的企业提供了可靠的决策依据。书中全方位比较了关系型数据库与NoSQL数据库的异同；分别以Riak、MongoDB、Cassandra和Neo4J为代表，详细讲解了键值数据库、文档数据库、列族数据库和图数据库这4大类NoSQL数据库的优劣势、用法和适用场合；深入探讨了实现NoSQL数据库系统的各种细节，以及与关系型数据库的混用。

* [《数据密集型应用系统设计》](https://book.douban.com/subject/30329536/)  
全面介绍现代数据系统的设计原理，涵盖数据模型、存储引擎、复制、分区、事务、分布式一致性以及批处理与流处理，帮助理解如何构建可靠、可扩展、易维护的应用。

### 编译原理
* [《编译原理》](https://book.douban.com/subject/3296317/)  
本书是编译领域无可替代的经典著作，被广大计算机专业人士誉为“龙书”。本书全面、深入地探讨了编译器设计方面的重要主题，包括词法分析、语法分析、语法制导定义和语法制导翻译、运行时刻环境、目标代码生成、代码优化技术、并行性检测以及过程间分析技术，并在相关章节中给出大量的实例。

### 数据结构&算法
* [《数据结构与算法分析：C语言描述》](https://book.douban.com/subject/1139426/)  
本书是《Data Structures and Algorithm Analysis in C》一书第2版的简体中译本，原书曾被评为20世纪顶尖的30部计算机著作之一。在本书中，作者更加精炼并强化了他对算法和数据结构方面创新的处理方法。通过C程序的实现，着重阐述了抽象数据类型的概念，并对算法的效率、性能和运行时间进行了分析。

* [《数据结构与算法分析：Java语言描述（原书第3版）》](https://book.douban.com/subject/26745780/)  
本书是国外数据结构与算法分析方面的经典教材，使用卓越的Java编程语言作为实现工具讨论了数据结构（组织大量数据的方法）和算法分析（对算法运行时间的估计）。 随着计算机速度的不断增加和功能的日益强大，人们对有效编程和算法分析的要求也不断增长。本书把算法分析与最有效率的Java程序的开发有机地结合起来，深入分析每种算法，内容全面、缜密严格，并细致讲解精心构造程序的方法。

* [《数据结构（C语言版）》](https://book.douban.com/subject/1886174/)  
《数据结构》(C语言版)针对采用ANSI C实现数据结构进行了全面的描述和深入的讨论。书中详细讨论了栈、队列、链表以及查找结构、高级树结构等功能，对裴波那契堆、伸展树、红黑树、2-3树、2-3-4树、二项堆、最小-最大堆、双端堆等新的数据结构进行了有效分析。

* [《数据结构（C语言版） 严蔚敏》](https://book.douban.com/subject/2024655/)  
本书是为“数据结构”课程编写的教材，也可作为学习数据结构及其算法的C程序设计的参数教材。
本书的前半部分从抽象数据类型的角度讨论各种基本类型的数据结构及其应用；后半部分主要讨论查找和排序的各种实现方法及其综合分析比较。

* [《算法导论》](https://book.douban.com/subject/20432061/)  
本书将严谨性和全面性融为一体，深入讨论各类算法，并着力使这些算法的设计和分析能为各个层次的读者接受。

* [《算法》](https://book.douban.com/subject/19952400/)  
本书是算法领域经典的参考书，涵盖所有程序员必须掌握的50种算法，全面介绍了关于算法和数据结构的必备知识，并特别针对排序、搜索、图处理和字符串处理进行了论述。

### 设计模式
* [《设计模式：可复用面向对象软件的基础》](https://book.douban.com/subject/1052241/)  
本书是引导读者走出软件设计迷宫的指路明灯，凝聚了软件开发界几十年设计经验的结晶。四位顶尖的面向对象领域专家精心选取了具有价值的设计实践，加以分类整理和命名，并用简洁而易于重用的形式表达出来。本书已经成为面向对象技术人员的圣经和词典，书中定义的23个模式逐渐成为开发界技术交流所必备的基础知识和语汇。

* [《Head First 设计模式》](https://book.douban.com/subject/2243615/)  
《O'Reilly：Head First设计模式（中文版）》趋近完美，因为它在提供专业知识的同时，仍然具有相当高的可读性。

* [《大话设计模式》](https://book.douban.com/subject/2334288/)  
本书是准备攀登面向对象编程高峰朋友们的引路人和提携者，是学习、体会和领悟了众多大师智慧结晶后的图书作品，是你深入理解和感受GoF的《设计模式》及其它大师作品的必备书籍。本书通篇都是以情景对话的形式，用多个小故事或编程示例来组织讲解GoF总结的23个设计模式。

### 软件工程
* [《软件工程：实践者的研究方法（原书第8版）》](https://book.douban.com/subject/26918148/)  
本书自 1982 年发行第 1 版以来，一直受到软件工程界的高度重视，是高等院校软件工程课程的重要教学参考书，全面而系统地介绍了软件工程的概念、原则、方法和工具。

* [《软件工程》](https://book.douban.com/subject/6109617/)  
本书是系统介绍软件工程理论的经典教材，自1982年初版以来，随着软件工程学科的发展不断更新版本，影响了一代又一代软件工程人才，对学科的发展建设也产生了积极影响。全书分四部分完整讨论了软件工程的各级段内容，是软件工程和系统工程专业本科和研究生的优秀教材，也是软件工程师必备的参考书籍。

* [《面向对象分析与设计》](https://book.douban.com/subject/3892590/)  
本书是一本注重实效的书，面向架构师和软件开发者等软件工程实践者的实际需要，通过大量例子说明了基本概念，解释了方法，并展示了在不同领域的成功应用。

* [《深入浅出面向对象分析与设计》](https://book.douban.com/subject/3530721/)  
本书将告诉你如何分析、设计以及撰写真正面向对象的软件；容易重用、好维护、可扩展的软件；不再使你心碎的软件；让你增添新功能而不会破坏旧机制的软件。

### 数字图像处理
* [《数字图像处理》](https://book.douban.com/subject/6434627/)  
本书是数字图像处理领域的杰作。

* [《图像处理、分析与机器视觉》](https://book.douban.com/subject/5921462/)  
本书是为计算机专业图像处理、图像分析和机器视觉课程编写的教材。书中针对图像处理、图像分析和机器视觉领域的有关原理与技术展开了广泛而深入的讨论，包括图像预处理、图像分割、形状表示与描述、物体识别与图像理解、三维视觉、数学形态学图像处理技术、离散图像变换、图像压缩、纹理描述、运动分析等。

* [《数字图像处理：MATLAB》](https://book.douban.com/subject/26344083/)  
本书是图像处理基础理论论述同以MATLAB为主要工具的软件实践方法相对照的第一本书，书中集成了冈萨雷斯和伍兹所著的《数字图像处理》一书中重要的原文材料和MathWorks公司的图像处理工具箱。本书的特色在于重点强调怎样通过开发新代码来加强这些软件工具。本书在介绍MATLAB编程基础知识之后，讲述了图像处理的主干内容，包括灰度变换、线性和非线性空间滤波、频率域滤波、图像复原与重建、彩色图像处理、图像压缩、图像分割、区域和边界表示与描述。

### 计算机图形学
* [《计算机图形学》](https://book.douban.com/subject/26403265/)  
本书是一本经典著作，全面系统地讲解了计算机图形学的基本概念和相关技术。

* [《计算机图形学》](https://book.douban.com/subject/3129340/)  
本书与大多数传统的计算机图形学教材不同，它仅简要介绍交互式计算机图形学方面的基本知识，主要侧重于介绍计算机图形学在数学及其他科学领域的应用，解决实际问题。

* [《计算机图形学》](https://book.douban.com/subject/3561816/)  
本书通过最能代表技术发展状况的示例综合介绍了计算机图形学方面的原则和技巧，书中对每个概念都进行了详细介绍，阐述了其背后的数学原理，并给出了用OpenGL实现的代码以及实现结果展示。

* [《OpenGL编程指南》](https://book.douban.com/subject/26220248/)  
本书清晰地讲解了OpenGL的相关功能与技术，包括几何对象顶点的传递、细分，几何着色器中的几何变换，通过片元着色器来操作像素和纹理贴图，以及基于帧缓存对象和计算着色器的先进数据操作技术。

* [《OpenGL超级宝典》](https://book.douban.com/subject/10774590/)  
本书是OpenGL及3D图形编程最好的入门指南，涵盖了使用最新版本的OpenGL进行编程所需要的主要知识。

### Linux
* [《深入理解LINUX内核》](https://book.douban.com/subject/2287506/)  
本书指导你对内核中使用的最重要的数据结构、算法和程序设计诀窍进行一次遍历。通过对表面特性的探究，作者给那些想知道自己机器工作原理的人提供了颇有价值的见解。

* [《深入Linux内核架构》](https://book.douban.com/subject/4843567/)  
本书讨论了Linux内核的概念、结构和实现。

* [《Linux程序设计》](https://book.douban.com/subject/4831448/)  
本书是Linux程序设计领域的经典名著，以简单易懂、内容全面和示例丰富而受到广泛好评。

* [《Linux内核设计与实现》](https://book.douban.com/subject/6097773/)  
本书详细描述了Linux内核的主要子系统和特点，包括Linux内核的设计、实现和接口。

* [《Linux/Unix设计思想》](https://book.douban.com/subject/7564417/)    
本书将Linux的开发方式与Unix的原理有效地结合起来，总结出Linux与Unix软件开发中的设计原则。

* [《鸟哥的Linux私房菜：基础学习篇（第四版）》](https://book.douban.com/subject/30359954/)  
本书是最具知名度的Linux入门书《鸟哥的Linux私房菜基础学习篇》的最新版，全面而详细地介绍了Linux操作系统。本书内容丰富全面，基本概念的讲解非常细致，深入浅出。各种功能和命令的介绍，都配以大量的实例操作和详尽的解析。本书是初学者学习Linux不可多得的一本入门好书。

* [《鸟哥的Linux私房菜：服务器架设篇(第3版)》](https://book.douban.com/subject/10794788/)     
您已有Linux基础，想要进一步学习服务器架设？还想了解如何维护与管理您的服务器？本书是您绝佳的选择。

* [《UNIX环境高级编程（第3版）》](https://book.douban.com/subject/25900403/)  
本书是被誉为UNIX编程“圣经”的Advanced Programming in the UNIX Environment一书的更新版。本书内容权威，概念清晰，阐述精辟，对于所有层次UNIX程序员都是一本不可或缺的参考书。

### Android
* [《第一行代码：Android（第3版）》](https://book.douban.com/subject/34996842/)  
本书被广大 Android 开发者誉为「Android 学习第一书」，系统全面、循序渐进地介绍了 Android 开发的必备知识、经验和技巧。第 3 版改用 Kotlin 讲解。

* [《Kotlin实战》](https://book.douban.com/subject/27093660/)  
由 JetBrains Kotlin 团队成员撰写，系统讲解 Kotlin 的语法与特性，以及如何在实际项目中使用 Kotlin。

* [《深入理解Kotlin协程》](https://book.douban.com/subject/35094136/)  
深入讲解 Kotlin 协程的概念、实现原理与使用方法。

* [《Effective Kotlin》](https://book.douban.com/subject/35341362/)  
总结编写安全、易读、高效的 Kotlin 代码的最佳实践（英文版）。

* [《Android开发艺术探索》](https://book.douban.com/subject/26599538/)  
本书是一本Android进阶类书籍，采用理论、源码和实践相结合的方式来阐述高水准的Android应用开发要点。

* [《Android源码设计模式解析与实战》](https://book.douban.com/subject/26644935/)    
本书从Android源码的角度由浅入深地剖析设计模式的运用，让工程师们把设计与模式重视起来，提升自己的设计能力与代码质量。

* [《深入理解Android内核设计思想（第2版）》](https://book.douban.com/subject/27074612/)  
本书从操作系统的基础知识入手，全面剖析进程/线程、内存管理、Binder机制、GUI显示系统、多媒体管理、输入系统等核心技术在Android中的实现原理。

* [《Android进阶解密》](https://book.douban.com/subject/30358046/)  
从源码角度深入解析 Android 系统启动、四大组件的工作过程、ClassLoader、热修复与插件化等原理。


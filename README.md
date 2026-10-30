Android Notes
==

English | [简体中文](README-CN.md)

A curated list of official documentation, open-source libraries, blogs, communities and classic books for Android development.

> Last updated: 2026-10-29. All links were checked when this list was updated; unmaintained, archived or unreachable entries have been removed. Many of the blogs, communities and books are in Chinese.

Contents
--
> * [Part 1: Frameworks](#part-1-frameworks)
>   * [Official Guides and Samples](#official-guides-and-samples)
>   * [Kotlin and Coroutines](#kotlin-and-coroutines)
>   * [Jetpack Compose and UI](#jetpack-compose-and-ui)
>   * [Cross-Platform](#cross-platform)
>   * [Jetpack Architecture Components](#jetpack-architecture-components)
>   * [Image Loading](#image-loading)
>   * [Networking](#networking)
>   * [Databases](#databases)
>   * [JSON](#json)
>   * [Dependency Injection](#dependency-injection)
>   * [Reactive Programming](#reactive-programming)
>   * [On-Device AI and LLMs](#on-device-ai-and-llms)
>   * [Build and Performance](#build-and-performance)
>   * [Crash Reporting](#crash-reporting)
>   * [Testing](#testing)
>   * [Charts](#charts)
>   * [Logging](#logging)
>   * [Plugins and Hotfix](#plugins-and-hotfix)
>   * [New Platforms and Capabilities](#new-platforms-and-capabilities)
> * [Part 2: Blogs and Communities](#part-2-blogs-and-communities)
>   * [Personal Blogs](#personal-blogs)
>   * [Team Blogs](#team-blogs)
>   * [Communities](#communities)
>   * [Newsletters](#newsletters)
> * [Part 3: Books](#part-3-books)
>   * [Computer Science Fundamentals](#computer-science-fundamentals)
>   * [Operating Systems](#operating-systems)
>   * [Computer Architecture](#computer-architecture)
>   * [Computer Networks](#computer-networks)
>   * [Databases](#databases-1)
>   * [Compilers](#compilers)
>   * [Data Structures and Algorithms](#data-structures-and-algorithms)
>   * [Design Patterns](#design-patterns)
>   * [Software Engineering](#software-engineering)
>   * [Digital Image Processing](#digital-image-processing)
>   * [Computer Graphics](#computer-graphics)
>   * [Linux](#linux)
>   * [Android](#android)


Part 1: Frameworks
--
### Official Guides and Samples
* [Guide to App Architecture](https://developer.android.com/topic/architecture) -- the officially recommended layered architecture and best practices
* [Now in Android](https://github.com/android/nowinandroid) -- a complete official sample app built with Kotlin, Compose and modern architecture
* [architecture-samples](https://github.com/android/architecture-samples) -- official architecture samples
* [compose-samples](https://github.com/android/compose-samples) -- official Compose samples
* [Android Courses](https://developer.android.com/courses)
* [Android Versions and Behavior Changes](https://developer.android.com/about/versions) -- new features and migration requirements of each release

### Kotlin and Coroutines
* [Kotlin Documentation](https://kotlinlang.org/docs/home.html)
* [Kotlin on Android](https://developer.android.com/kotlin)
* [Kotlin Coroutines](https://developer.android.com/kotlin/coroutines) -- the official approach to asynchronous programming; source at [kotlinx.coroutines](https://github.com/Kotlin/kotlinx.coroutines)
* [Kotlin Flow](https://developer.android.com/kotlin/flow) -- asynchronous data streams, also a replacement for event buses such as EventBus
* [kotlinx-datetime](https://github.com/Kotlin/kotlinx-datetime) -- a multiplatform date and time library

### Jetpack Compose and UI
* [Jetpack Compose](https://developer.android.com/compose) -- the official declarative UI toolkit
* [Material Design 3](https://m3.material.io/) -- the design system; see [Material 3 in Compose](https://developer.android.com/develop/ui/compose/designsystems/material3)
* [Navigation 3](https://developer.android.com/guide/navigation/navigation-3) -- the next-generation navigation library for Compose
* [Edge-to-edge](https://developer.android.com/develop/ui/views/layout/edge-to-edge) -- drawing behind the system bars
* [View Binding](https://developer.android.com/topic/libraries/view-binding) -- replaces the unmaintained Butter Knife
* [Circuit](https://github.com/slackhq/circuit) -- a Compose-driven architecture from Slack
* [Lottie](https://lottie.airbnb.tech/) -- an animation library from Airbnb

### Cross-Platform
* [Kotlin Multiplatform](https://kotlinlang.org/docs/multiplatform.html) -- share Kotlin code across Android, iOS, desktop and web
* [Kotlin Multiplatform on Android](https://developer.android.com/kotlin/multiplatform)
* [Compose Multiplatform](https://kotlinlang.org/compose-multiplatform/) -- cross-platform Compose UI from JetBrains; source at [compose-multiplatform](https://github.com/JetBrains/compose-multiplatform)

### Jetpack Architecture Components
* [Room](https://developer.android.com/training/data-storage/room) -- the official SQLite ORM
* [DataStore](https://developer.android.com/topic/libraries/architecture/datastore) -- replaces SharedPreferences
* [WorkManager](https://developer.android.com/develop/background-work/background-tasks/persistent) -- reliable background work scheduling
* [Paging 3](https://developer.android.com/topic/libraries/architecture/paging/v3-overview) -- paged data loading

### Image Loading
* [Coil](https://coil-kt.github.io/coil/) -- Kotlin-first, supports Compose and Kotlin Multiplatform
* [Glide](https://github.com/bumptech/glide)
* [Fresco](https://frescolib.org/) -- the repository has moved to [meta/fresco](https://github.com/meta/fresco)

### Networking
* [OkHttp](https://lysine.dev/okhttp/) -- the repository has moved to [lysine-dev/okhttp](https://github.com/lysine-dev/okhttp)
* [Retrofit](https://lysine.dev/retrofit/) -- the repository has moved to [lysine-dev/retrofit](https://github.com/lysine-dev/retrofit)
* [Ktor](https://ktor.io/) -- a Kotlin multiplatform networking framework from JetBrains
* [Wire](https://github.com/square/wire) -- gRPC and Protocol Buffers

### Databases
* [Room](https://developer.android.com/training/data-storage/room)
* [SQLDelight](https://sqldelight.github.io/sqldelight/) -- generates type-safe Kotlin APIs from SQL, with multiplatform support
* [ObjectBox](https://github.com/objectbox/objectbox-java) -- an object database with on-device vector search

### JSON
* [kotlinx.serialization](https://kotlinlang.org/docs/serialization.html) -- the official Kotlin serialization library
* [Moshi](https://github.com/square/moshi)
* [Gson](https://github.com/google/gson)
* [Jackson](https://github.com/FasterXML/jackson)
* [fastjson2](https://github.com/alibaba/fastjson2) -- replaces the archived fastjson

### Dependency Injection
* [Hilt](https://developer.android.com/training/dependency-injection/hilt-android) -- officially recommended, built on Dagger
* [Dagger](https://dagger.dev/)
* [Koin](https://insert-koin.io/) -- a lightweight Kotlin dependency injection framework
* [Metro](https://github.com/ZacSweers/metro) -- a compile-time, multiplatform dependency injection framework for Kotlin
* [kotlin-inject](https://github.com/evant/kotlin-inject)

### Reactive Programming
* [Kotlin Flow](https://developer.android.com/kotlin/flow)
* [RxJava](https://github.com/ReactiveX/RxJava)
* [RxAndroid](https://github.com/ReactiveX/RxAndroid)

### On-Device AI and LLMs
* [AI on Android](https://developer.android.com/ai)
* [Gemini Nano](https://developer.android.com/ai/gemini-nano) -- the Gemini model that runs on device
* [ML Kit GenAI APIs](https://developers.google.com/ml-kit/genai) -- summarization, rewriting, image description and more, powered by on-device models
* [Firebase AI Logic](https://firebase.google.com/docs/ai-logic) -- call cloud Gemini models directly from your app
* [LiteRT](https://developers.google.com/edge/litert) -- the successor to TensorFlow Lite, an on-device runtime for machine learning and generative AI
* [MediaPipe](https://developers.google.com/edge/mediapipe/solutions/guide) -- on-device machine learning solutions
* [Koog](https://github.com/JetBrains/koog) -- an open-source Kotlin AI agent framework from JetBrains
* [ai-samples](https://github.com/android/ai-samples) -- official AI samples
* [Gemini in Android Studio](https://developer.android.com/studio/gemini/overview) -- the AI coding assistant built into Android Studio

### Build and Performance
* [KSP](https://github.com/google/ksp) -- Kotlin Symbol Processing, the replacement for kapt; see the [migration guide](https://developer.android.com/build/migrate-to-ksp)
* [Version catalogs](https://developer.android.com/build/migrate-to-catalogs) -- manage dependency versions in one place
* [R8 app optimization](https://developer.android.com/topic/performance/app-optimization/enable-app-optimization) -- code shrinking, obfuscation and optimization
* [Baseline Profiles](https://developer.android.com/topic/performance/baselineprofiles/overview) -- improve startup and runtime performance
* [Macrobenchmark](https://developer.android.com/topic/performance/benchmarking/macrobenchmark-overview) -- benchmark startup, scrolling and other scenarios
* [Perfetto](https://perfetto.dev/) -- system-wide performance tracing and analysis
* [LeakCanary](https://square.github.io/leakcanary/) -- memory leak detection
* [KOOM](https://github.com/KwaiAppTeam/KOOM) -- OOM monitoring from Kuaishou
* [Support 16 KB page sizes](https://developer.android.com/guide/practices/page-sizes)

### Crash Reporting
* [Firebase Crashlytics](https://firebase.google.com/docs/crashlytics)
* [Sentry](https://github.com/getsentry/sentry-java)
* [ACRA](https://github.com/ACRA/acra)

### Testing
* [Test apps on Android](https://developer.android.com/training/testing)
* [Testing Compose layouts](https://developer.android.com/develop/ui/compose/testing)
* [Robolectric](https://github.com/robolectric/robolectric) -- run Android tests on the JVM
* [MockK](https://github.com/mockk/mockk) -- a mocking library for Kotlin
* [Turbine](https://github.com/cashapp/turbine) -- a testing library for Kotlin Flow
* [Paparazzi](https://github.com/cashapp/paparazzi) -- screenshot tests without a device
* [Roborazzi](https://github.com/takahirom/roborazzi) -- screenshot tests based on Robolectric

### Charts
* [Vico](https://github.com/patrykandpatrick/vico) -- a chart library with Compose Multiplatform support
* [MPAndroidChart](https://github.com/PhilJay/MPAndroidChart)

### Logging
* [Timber](https://github.com/JakeWharton/timber)
* [Logger](https://github.com/orhanobut/logger)

### Plugins and Hotfix
* [Tinker](https://github.com/Tencent/tinker) -- a hotfix solution from Tencent
* [Shadow](https://github.com/Tencent/Shadow) -- a zero-reflection, fully dynamic plugin framework from Tencent

### New Platforms and Capabilities
* [Android XR](https://developer.android.com/develop/xr)
* [Credential Manager](https://developer.android.com/identity/credential-manager) -- a unified API for passkeys, passwords and federated sign-in

Part 2: Blogs and Communities
--
### Personal Blogs
* [Luo Shengyang's Android Journey](https://blog.csdn.net/luoshengyang)
* [Trinea](https://www.trinea.cn/)
* [Guo Lin](https://blog.csdn.net/guolin_blog)
* [Xia Anming](https://blog.csdn.net/xiaanming)
* [Hongyang](https://blog.csdn.net/lmj623565791)
* [Ren Yugang](https://blog.csdn.net/singwhatiwanna)
* [stormzhang](https://stormzhang.com/)
* [Ma Tianyu (litesuits)](https://github.com/litesuits)
* [Ruan Yifeng's Weblog](https://www.ruanyifeng.com/blog/)
* [Zhang Tao - Open Source Lab](http://blog.kymjs.com/)
* [Xie Quan (SELF)](https://xiequan.info/)
* [He Honghui (Mr.Simple)](https://blog.csdn.net/bboyfeiyu)
* [Droidyue](https://droidyue.com/)
* [eclipse_xu](https://blog.csdn.net/eclipsexys)
* [Zimo's Blog](https://blog.csdn.net/ElinaVampire)
* [wwj_748](https://blog.csdn.net/wwj_748)
* [AigeStudio](https://blog.csdn.net/aigestudio)
* [Yusong MOMO](https://www.xuanyusong.com/)
* [Bao Jianqiang](https://blog.csdn.net/jspandasp)
* [Deng Fanping](https://blog.csdn.net/innost)
* [Piasy](https://blog.piasy.com/)
* [Yuan Bin](https://blog.csdn.net/qibin0506)
* [Zhao Si](https://blog.csdn.net/jiangwei0910410003)
* [weishu](https://weishu.me/)
* [Yan Zhenjie](https://blog.csdn.net/yanzhenjie1003)
* [mynameishuangshuai](https://blog.csdn.net/mynameishuangshuai)
* [markzhai](http://blog.zhaiyifan.cn/)
* [ns_code](https://blog.csdn.net/ns_code)
* [qianxudetianxia](https://www.cnblogs.com/qianxudetianxia)
* [yanbober](https://blog.csdn.net/yanbober)
* [diygreen](https://www.jianshu.com/u/0ad0a0afc409)
* [VERYYOUNG](http://veryyoung.me/)
* [Zuo Fei](https://blog.csdn.net/baimafujinji)
* [Frodo](http://frodoking.github.io/)
* [Lading Wu](https://www.jianshu.com/u/1d8042233f67)
* [Carson_Ho](https://blog.csdn.net/carson_ho)
* [Gityuan](http://gityuan.com/)
* [GcsSloop](https://www.gcssloop.com/)
* [frank (briblue)](https://blog.csdn.net/briblue)
* [Gavin Liu](https://www.gavinliu.cn/)
* [SpikeKing](https://www.jianshu.com/u/e2b4dd6d3eb4)
* [Wang Yeming](https://wangyeming.github.io/)
* [Coder-Pig](https://blog.csdn.net/coder_pig)
* [Android Performance](https://www.androidperformance.com/)
* [Ouyang Peng](https://blog.csdn.net/ouyang_peng)
* [heqiangfly](https://www.heqiangfly.com/)
* [Juejin user 1503787635450584](https://juejin.cn/user/1503787635450584)
* [bugstack](https://bugstack.cn/)
* [Fenfei Security](http://91fans.com.cn/)
* [javagame.top](https://www.javagame.top/index.html)

### Team Blogs
* [Android Developers Blog](https://android-developers.googleblog.com/) -- the official Android blog
* [Kotlin Blog](https://blog.jetbrains.com/kotlin/) -- the official Kotlin blog
* [Meituan Tech](https://tech.meituan.com/)
* [Tencent AlloyTeam](http://www.alloyteam.com/)
* [Square Developer Blog](https://developer.squareup.com/blog/)
* [Meta Engineering](https://engineering.fb.com/)
* [Tencent Game Security Lab](https://gslab.qq.com/)

### Communities
* [CSDN](https://www.csdn.net/)
* [cnblogs](https://www.cnblogs.com/)
* [51CTO](http://www.51cto.com/)
* [OSCHINA](https://www.oschina.net/)
* [CocoaChina](http://www.cocoachina.com/)
* [open-open](https://www.open-open.com/)
* [Juejin](https://juejin.cn/)
* [IBM Developer](https://developer.ibm.com/)
* [SegmentFault](https://segmentfault.com/)
* [InfoQ China](https://www.infoq.cn/)
* [ChinaUnix](https://blog.chinaunix.net/)
* [ITPUB](https://blog.itpub.net/)
* [toutiao.io](https://toutiao.io/)
* [Runoob](https://www.runoob.com/)
* [V2EX](https://www.v2ex.com/)
* [FreeBuf](https://www.freebuf.com/)
* [Google Developers China (Youku)](http://i.youku.com/i/UMjczOTc0NDkzNg==)
* [GDG China](https://www.chinagdg.com/)
* [Xiaozhuanlan](https://xiaozhuanlan.com/)

### Newsletters
* [Android Weekly](https://androidweekly.net/)
* [Kotlin Weekly](https://kotlinweekly.net/)
* [Android Weekly (Chinese)](https://androidweekly.io/)
* [Ping An Fintech Mobile Weekly](https://www.jianshu.com/notebooks/2983917/latest)

Part 3: Books
--
> The links point to the Douban pages of the Chinese editions.

### Computer Science Fundamentals
* [Foundations of Computer Science](https://book.douban.com/subject/1142213/)  
An introductory textbook covering every area of computer science, focusing on concepts rather than mathematical models, with many figures and examples.

* [Computer Systems: A Programmer's Perspective](https://book.douban.com/subject/5333562/)  
Explains the essential concepts of computer systems from a programmer's point of view, and how they affect the correctness, performance and usefulness of programs.

### Operating Systems
* [Modern Operating Systems](https://book.douban.com/subject/3852290/)  
A classic on the principles of operating systems: processes, threads, memory management, file systems, I/O, deadlocks, security, multimedia, virtualization and OS design.

* [Operating Systems: Internals and Design Principles](https://book.douban.com/subject/5064311/)   
Covers the concepts, principles and methods of operating systems, and the nature and characteristics of modern operating systems.

### Computer Architecture
* [Computer Architecture: A Quantitative Approach](https://book.douban.com/subject/20452387/)   
The definitive book on computer architecture: design fundamentals, instruction sets, pipelining and instruction-level parallelism, memory hierarchy, interconnection networks and multiprocessors.

* [Computer Organization and Design: The Hardware/Software Interface](https://book.douban.com/subject/2110638/)  
A classic textbook on computer organization that shows the relationship between hardware and software.

* [Computer Organization and Architecture: Designing for Performance](https://book.douban.com/subject/6398113/)  
Discusses the principles of computer organization and architecture using the Intel x86 and ARM processor families as examples.

* [Computer Organization and Architecture](https://book.douban.com/subject/1881545/)  
Covers digital logic, data representation, assembly-level organization, memory, interfaces and communication, multiprocessors, performance and distributed systems.

* [Computer Organization and Architecture (Pentium 4 / PowerPC edition)](https://book.douban.com/subject/1737686/)  
Relates performance issues of modern computer systems to the principles of computer organization, using the Intel Pentium 4 and IBM/Motorola PowerPC as case studies.

### Computer Networks
* [Computer Networks](https://book.douban.com/subject/10510747/)  
One of the most widely used networking textbooks, covering the protocol stack bottom-up with many Internet examples, plus wireless, 3G, RFID, CDN, P2P and streaming.

* [Computer Networking: A Top-Down Approach](https://book.douban.com/subject/26176870/)  
The textbook that pioneered teaching network principles and protocols top-down.

* [Understanding Computer Networks](https://book.douban.com/subject/20560942/)  
A systematic and in-depth look at network architecture, how networks work and how protocols are implemented.

* [TCP/IP Illustrated, Volume 1: The Protocols](https://book.douban.com/subject/1088054/)  
A complete and detailed guide to the TCP/IP protocols at every layer and how they behave on different operating systems.

* [TCP/IP Illustrated, Volume 2: The Implementation](https://book.douban.com/subject/1087767/)  
A detailed walkthrough of how TCP/IP is implemented.

* [TCP/IP Illustrated, Volume 3: TCP for Transactions, HTTP, NNTP, and the UNIX Domain Protocols](https://book.douban.com/subject/1058634/)  
The continuation of the series, covering T/TCP, HTTP, NNTP and UNIX domain protocols.

* [TCP/IP Protocol Suite](https://book.douban.com/subject/5386194/)  
A classic introduction to the TCP/IP protocol suite.

* [HTTP: The Definitive Guide](https://book.douban.com/subject/10746113/)  
Explains how HTTP works, how to build web applications with it, and how to implement clients and servers correctly.

### Databases
* [Database System Concepts](https://book.douban.com/subject/10548379/)  
A cornerstone book for building a solid foundation in database theory.

* [Database Systems: The Complete Book](https://book.douban.com/subject/4838430/)  
One of the most comprehensive books on implementing database systems, used in Stanford's database course series.

* [High Performance MySQL](https://book.douban.com/subject/23008813/)  
A classic and influential book on MySQL.

* [The Definitive Guide to MySQL 5](https://book.douban.com/subject/1909003/)  
A reference for MySQL administrators and developers.

* [MongoDB: The Definitive Guide](https://book.douban.com/subject/25798102/)  
Covers MongoDB's document model, queries, indexing, aggregation, monitoring, security, backup and sharding.

* [Redis Design and Implementation](https://book.douban.com/subject/25900156/)  
A thorough description of how Redis works internally.

* [NoSQL Distilled](https://book.douban.com/subject/25662138/)  
Compares relational and NoSQL databases, and explains key-value, document, column-family and graph databases using Riak, MongoDB, Cassandra and Neo4j.

### Compilers
* [Compilers: Principles, Techniques, and Tools](https://book.douban.com/subject/3296317/)  
The "Dragon Book": lexical analysis, parsing, syntax-directed translation, runtime environments, code generation, optimization, parallelism detection and interprocedural analysis.

### Data Structures and Algorithms
* [Data Structures and Algorithm Analysis in C](https://book.douban.com/subject/1139426/)  
A classic that explains abstract data types and analyzes the efficiency and running time of algorithms, with implementations in C.

* [Data Structures and Algorithm Analysis in Java](https://book.douban.com/subject/3351237/)  
The Java edition, combining algorithm analysis with the development of efficient Java programs.

* [Fundamentals of Data Structures in C](https://book.douban.com/subject/1886174/)  
Covers stacks, queues, linked lists, search structures and advanced trees and heaps in ANSI C.

* [Data Structures (C edition) by Yan Weimin](https://book.douban.com/subject/2024655/)  
A widely used Chinese textbook covering basic data structures, searching and sorting.

* [Introduction to Algorithms](https://book.douban.com/subject/20432061/)  
A rigorous and comprehensive treatment of the design and analysis of algorithms.

* [Algorithms](https://book.douban.com/subject/19952400/)  
A classic reference covering the essential algorithms and data structures, with a focus on sorting, searching, graphs and strings.

### Design Patterns
* [Design Patterns: Elements of Reusable Object-Oriented Software](https://book.douban.com/subject/1052241/)  
The "Gang of Four" book that defined the 23 classic design patterns.

* [Head First Design Patterns](https://book.douban.com/subject/2243615/)  
Professional knowledge presented in a highly readable way.

* [Big Talk Design Patterns](https://book.douban.com/subject/2334288/)  
A Chinese book that explains the 23 GoF patterns through dialogues, stories and examples.

### Software Engineering
* [Software Engineering: A Practitioner's Approach](https://book.douban.com/subject/6047742/)  
A highly regarded reference on the concepts, principles, methods and tools of software engineering since 1982.

* [Software Engineering](https://book.douban.com/subject/6109617/)  
A classic textbook on software engineering theory, continuously updated since 1982.

* [Object-Oriented Analysis and Design with Applications](https://book.douban.com/subject/3892590/)  
A practical book for architects and developers, with many examples across different domains.

* [Head First Object-Oriented Analysis and Design](https://book.douban.com/subject/3530721/)  
How to analyze, design and write object-oriented software that is reusable, maintainable and extensible.

### Digital Image Processing
* [Digital Image Processing](https://book.douban.com/subject/6434627/)  
A masterpiece in the field of digital image processing.

* [Image Processing, Analysis, and Machine Vision](https://book.douban.com/subject/5921462/)  
A textbook covering preprocessing, segmentation, shape description, object recognition, 3D vision, morphology, transforms, compression, texture and motion analysis.

* [Digital Image Processing Using MATLAB](https://book.douban.com/subject/26344083/)  
Pairs image processing theory with practical MATLAB implementations.

### Computer Graphics
* [Computer Graphics (C version)](https://book.douban.com/subject/26403265/)  
A classic that covers the basic concepts and techniques of computer graphics.

* [Computer Graphics (mathematical applications)](https://book.douban.com/subject/3129340/)  
Briefly introduces interactive graphics and focuses on applying graphics to mathematics and other sciences.

* [Computer Graphics (with OpenGL)](https://book.douban.com/subject/3561816/)  
Explains the principles and techniques of computer graphics with the underlying math and OpenGL code.

* [OpenGL Programming Guide](https://book.douban.com/subject/26220248/)  
Covers vertex processing, tessellation, geometry shaders, fragment shaders, textures, framebuffer objects and compute shaders.

* [OpenGL SuperBible](https://book.douban.com/subject/10774590/)  
One of the best introductions to OpenGL and 3D graphics programming.

### Linux
* [Understanding the Linux Kernel](https://book.douban.com/subject/2287506/)  
A tour of the most important data structures, algorithms and programming techniques used in the kernel.

* [Professional Linux Kernel Architecture](https://book.douban.com/subject/4843567/)  
Discusses the concepts, structure and implementation of the Linux kernel.

* [Beginning Linux Programming](https://book.douban.com/subject/4831448/)  
A classic on Linux programming, easy to follow and full of examples.

* [Linux Kernel Development](https://book.douban.com/subject/6097773/)  
Describes the main subsystems of the Linux kernel, their design, implementation and interfaces.

* [Linux and the Unix Philosophy](https://book.douban.com/subject/7564417/)    
Summarizes the design principles of Linux and Unix software development.

* [Vbird's Linux Book: Basic Learning (3rd edition)](https://book.douban.com/subject/4889838/)  
One of the best-known introductions to Linux, with detailed explanations and many hands-on examples.

* [Vbird's Linux Book: Server Setup (3rd edition)](https://book.douban.com/subject/10794788/)     
For readers who know Linux basics and want to set up and maintain servers.

* [Advanced Programming in the UNIX Environment](https://book.douban.com/subject/1788421/)  
Known as the "bible" of UNIX programming, an indispensable reference for UNIX programmers.

### Android
* [The Definitive Guide to Android Development](https://book.douban.com/subject/25741542/)  
A comprehensive book on Android app development.

* [The First Line of Code](https://book.douban.com/subject/26915433/)  
Known among Chinese developers as "the first book for learning Android", a step-by-step introduction.

* [Android Kernel Analysis](https://book.douban.com/subject/6811238/)  
Analyzes the window manager, activity manager, input method framework and build system of Android.

* [Exploring the Art of Android Development](https://book.douban.com/subject/26599538/)  
An advanced Android book combining theory, source code and practice.

* [Design Patterns in Android Source Code](https://book.douban.com/subject/26644935/)    
Analyzes how design patterns are used in the Android source code.

* [Inside Android 5.0](https://book.douban.com/subject/26377840/)    
Analyzes the principles and implementation of the main frameworks of Android 5.0.

* [Understanding the Design of the Android Kernel](https://book.douban.com/subject/25921329/)   
Covers processes and threads, memory management, Binder, the display system, multimedia and input in Android.

* [Android Software Security and Reverse Engineering](https://book.douban.com/subject/20556210/)    
Covers static analysis, dynamic debugging, cracking and anti-cracking techniques, and analysis of typical Android malware.

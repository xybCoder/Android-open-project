# Android 优秀开源项目汇总

-----


##  事件总线(订阅者模式)

通过发布/订阅事件解耦事件发送和接受，从而简化应用程序之间的通信

### **1.EventBus     作者 greenrobot**

项目地址：https://github.com/greenrobot/EventBus

原理剖析文档：https://github.com/greenrobot/EventBus#general-usage-and-api

特点：

1.  支持在不同类型的线程中处理订阅，包括发布所在线程，UI 线程、单一后台线程、异步线程
2.  支持事件优先级定义，支持优先级高的订阅者取消事件继续传递，支持粘性事件，是不是跟系统的有序广播、粘性广播很像
3.  不是基于 annotations
4.  性能更优
5.  体积小
6.  支持单例创建或创建多个对象
7.  支持根据事件类型订阅


### **2.Otto     开源组织 Square **

项目地址：https://github.com/square/otto
文档介绍：http://square.github.io/otto/



## 网络请求

### **1.Volley    开源组织 Google**

项目地址：https://android.googlesource.com/platform/frameworks/volley

文档介绍：http://commondatastorage.googleapis.com/io-2013/presentations/110%20-%20Volley-%20Easy,%20Fast%20Networking%20for%20Android.pdf

特点：

（1）库小，Google 维护，提供的网络通信库，使得网络请求更简单、更快速

### **2.okhttp    开源组织 Square**

项目地址：https://github.com/square/okhttp

文档介绍：http://square.github.io/okhttp/

特点：

1. 支持 SPDY( http://zh.wikipedia.org/wiki/SPDY )协议。SPDY 协议是 Google 开发的基于传输控制协议的应用层协议，通过压缩，多路复用(一个 TCP 链接传送网页和图片等资源)和优先级来缩短加载时间。
2. 如果 SPDY 不可用，利用连接池减少请求延迟
3. Gzip 压缩
4. Response 缓存减少不必要的请求

### **3.Retrofit   开源组织 Square**

项目地址：https://github.com/square/retrofit

文档介绍：http://square.github.io/retrofit/

特点：

（1）配合Rx.xxx系列使用代码更加简洁

### ** 4.Asynchronous Http Client for Android  **

项目地址：https://github.com/loopj/android-async-http

文档介绍：http://loopj.com/android-async-http/

特点：

1. 异步 Http 请求
2. 在匿名回调中处理请求结果
3. 在 UI 线程外进行 http 请求
4. 文件断点上传
5. 智能重试
6. 默认 gzip 压缩
7. 支持解析成 Json 格式
8. 可将 Cookies 持久化到 SharedPreferences

## 图片缓存

### **1.Android-Universal-Image-Loader**

项目地址：https://github.com/nostra13/Android-Universal-Image-Loader

原理剖析文档：Android-Universal-Image-Loader

特点：
1. 目前使用最广泛的图片缓存，支持主流图片缓存的绝大多数特性

### **2.picasso   开源组织 Square**

项目地址：https://github.com/square/picasso

文档介绍：http://square.github.io/picasso/

特点：

1. 可以自动检测 adapter 的重用并取消之前的下载
2. 图片变换
3. 可以加载本地资源
4. 可以设置占位资源
5. 支持 debug 模式

### **3.Cube ImageLoader  开源组织 阿里巴巴一淘**

项目地址：https://github.com/etao-open-source/cube-sdk

Demo 地址：https://github.com/liaohuqiu/cube-sdk/raw/master/cube-sdk-sample.apk

特点：
1. 综合了 Android-Universal-Image-Loader 和 square 等组件优点，简单易用，良好的中文文档支持

### **4.fresco  开源组织  Facebook **

项目地址：https://github.com/facebook/fresco

文档介绍：http://frescolib.org/

特点：

1. 两个内存缓存加上磁盘缓存构成了三级缓存
2. 支持流式，可以类似网页上模糊渐进式显示图片
3. 对多帧动画图片支持更好，如 Gif、WebP
4. 更多样的显示，如圆角、进度条、点击重试、自定义对焦点
5. 更多样的加载，如支持 EXIF、全面支持 WebP
6. 支持 Android 2.3+

### **5.Glide    作者 bumptech**

项目地址：https://github.com/bumptech/glide

特点：

1. GIF 动画的解码
2. 本地视频剧照的解码
3. 支持缩略图
4. Activity 生命周期的集成
5. 转码的支持
6. 动画的支持
7. OkHttp 和 Volley 的支持


## 数据库 

### **1.greenDAO  作者greenrobot**

Android Sqlite orm 的 db 工具类

项目地址：https://github.com/greenrobot/greenDAO

文档介绍：http://greendao-orm.com/documentation/

特点：

1. 性能佳
2. 简单易用的 API
3. 内存小好小
4. 库大小小


### **2.ActiveAndroid **

项目地址：https://github.com/pardom/ActiveAndroid

文档介绍：https://github.com/pardom/ActiveAndroid/wiki/_pages


## 响应式编程Rx.xx

学习Rx.java 资料：https://github.com/lzyzsd/Awesome-RxJava

### **1.RxJava    开源组织ReactiveX**

项目地址：https://github.com/ReactiveX/RxJava


### **2.RxAndroid     开源组织ReactiveX **

项目地址：https://github.com/ReactiveX/RxAndroid

特点：RxJava的Android拓展

### ** 3.rx-preferences **

项目地址： https://github.com/f2prateek/rx-preferences

特点：

1. 使SharedPreferences支持RxJava

### **4.RxBinding   作者JakeWharton**
项目地址：https://github.com/JakeWharton/RxBinding

特点：

1. 安卓UI控件的RxJava绑定API

### **5.xBus  作者 mcxiaoke**

项目地址：https://github.com/mcxiaoke/xBus

特点：

1. 简洁的EventBus实现

### **6.RxLifecycle 作者 trello**

项目地址：https://github.com/trello/RxLifecycle

特点：帮助使用了RxJava的安卓应用控制生命周期

### **7. sqlbrite  开源组织 square**

项目地址： https://github.com/square/sqlbrite

特点：支持RxJava的sqlite数据库


## 依赖注入 

通过依赖注入减少 View、服务、资源简化初始化，事件绑定等重复繁琐工作

### **1.AndroidAnnotations(Code Diet)**

项目地址：https://github.com/excilys/androidannotations

文档介绍：https://github.com/excilys/androidannotations/wiki

官网网址：http://androidannotations.org/

特点：

1. 依赖注入：包括 view，extras，系统服务，资源等等
2. 简单的线程模型，通过 annotation 表示方法运行在 ui 线程还是后台线程
3. 事件绑定：通过 annotation 表示 view 的响应事件，不用在写内部类
4. REST 客户端：定义客户端接口，自动生成 REST 请求的实现
5. 没有你想象的复杂：AndroidAnnotations 只是在在编译时生成相应子类
6. 不影响应用性能：仅 50kb，在编译时完成，不会对运行时有性能影响

### **2.butterknife  作者JakeWharton**

利用 annotation 帮你快速完成 View 的初始化，减少代码

项目地址：https://github.com/JakeWharton/butterknife

文档介绍：http://jakewharton.github.io/butterknife/

### **3.Dagger 开源组织square**

依赖注入，适用于 Android 和 Java

项目地址：https://github.com/square/dagger

原理剖析文档：Dagger

文档介绍：http://square.github.io/dagger/

### **4.Dagger2 开源组织Google**

项目地址：https://github.com/google/dagger

官网文档：http://google.github.io/dagger/

## RecyclerView

###　1.IndexRecyclerView 实现联系人的功能

1. 首字母悬浮在顶部。
2. 侧滑删除联系人。
3. 联系人索引。

项目地址：https://github.com/jiang111/IndexRecyclerView

效果图：

![icon](/images/art.gif)

### 2.RecyclerViewEnhanced

项目地址：https://github.com/nikhilpanju/RecyclerViewEnhanced

效果图：

![icon](/images/Demo.gif)

### 3.RecyclerViewUndoSwipe

项目地址：https://github.com/HoneyNeutrons/RecyclerViewUndoSwipe

效果图：

![icon](/images/687474703a2f2f696d6775722e636f6d2f523931554a716c2e676966.gif)

### 4.UltimateRecyclerView

项目地址：https://github.com/cymcsg/UltimateRecyclerView

效果图：

![icon](/images/687474703a2f2f692e67697068792e636f6d2f704c57484b734564566c734b412e676966.gif)![icon](/images/687474703a2f2f692e67697068792e636f6d2f62765534486357764d68656a6d2e676966.gif)![icon](/images/68747470733a2f2f627974656275636b65742e6f72672f6d61727368616c6368656e2f696d616765732f7261772f343462656231363231323163373139656134303934626437656131633966306364376465346330342f756c74696d61746572656379636c6572766965772f756c74.gif)

### 5.android-advancedrecyclerview

RecyclerView支持各种功能的库

项目地址：https://github.com/h6ah4i/android-advancedrecyclerview

### 6.SuperSLiM

RecyclerView 的一款layout manager，支持linear，grid以及staggered之间的互换.并支持sticky特性

项目地址：https://github.com/TonicArtos/SuperSLiM

效果图：

![icon](/images/68747470733a2f2f342e62702e626c6f6773706f742e636f6d2f2d657034364a4b70476138342f564a685831706c575743492f4141414141414141585a592f394131417272563361336b2f73313630302f5375706572534c694d2d44656d6f2d736d616c6c2e676966.gif)

### 7.recyclerview-animators

各种动画库， 添加 itemanimator 到 RecyclerView items

项目地址：https://github.com/wasabeef/recyclerview-animators

效果图：

![icon](/images/demo2.gif)![icon](/images/demo4.gif)

### 8.RecyclerViewSwipeDismiss

滑动删除的RecyclerView

项目地址：https://github.com/CodeFalling/RecyclerViewSwipeDismiss

效果图：

![icon](/images/RecyclerViewSwipeDismiss.gif)

### 9.Searchable RecyclerView

利用SearchView实现的RecyclerView搜索效果，并且充分利用了RecyclerView中的item animations 动画

项目地址：https://github.com/Wrdlbrnft/Searchable-RecyclerView-Demo

效果图：

![icon](/images/687474703a2f2f692e737461636b2e696d6775722e636f6d2f68747a30592e676966.gif)

### 10.EasyRecyclerViewSidebar

实现伦敦眼效果的LayoutManager

项目地址：https://github.com/CaMnter/EasyRecyclerViewSidebar

效果图：

![icon](/images/687474703a2f2f7777342e73696e61696d672e636e2f6c617267652f3030366c504563396777316633307662396d78767a6a333161793239386b30672e6a7067.jpg)![icon](/images/687474703a2f2f7777312e73696e61696d672e636e2f6c617267652f3030366c50456339677731663330763333717365646a33316179323938776d6e2e6a7067.jpg)

### 11.ItemTouchHelperDemo

使用ItemTouchHelper实现今日头条 网易新闻 的频道排序、频道移动

项目地址：https://github.com/YoKeyword/ItemTouchHelperDemo

效果图：

![icon](/images/687474703a2f2f75706c6f61642d696d616765732e6a69616e7368752e696f2f75706c6f61645f696d616765732f3933373835312d326466353066663938333364643338362e6769663f696d6167654d6f6772322f6175746f2d6f7269656e742f7374726970.gif)


## Adapter

### 1.BaseRecyclerViewAdapterHelper

1. 优化Adapter代码（减少百分之70%代码）
2. 添加点击item点击、长按事件、以及item子控件的点击事件
3. 添加加载动画（一行代码轻松切换5种默认动画）
4. 添加头部、尾部、下拉刷新、上拉加载（感觉又回到ListView时代）
5. 设置自定义的加载更多布局
6. 添加分组（随心定义分组头部）
7. 自定义不同的item类型（简单配置、无需重写额外方法）
8. 设置空布局（比Listview的setEmptyView还要好用！）
9. 添加拖拽item

项目地址：https://github.com/CymChad/BaseRecyclerViewAdapterHelper

效果图：

![icon](/images/chlid_click.gif)![icon](/images/animation.gif)![icon](/images/multiple_item.gif)|



### 2.FlexibleAdapter

一款强大的RecyclerView的adapter，支持ViewHolders动画，拖拽，滑动，取消, 伸缩等

项目地址：https://github.com/davideas/FlexibleAdapter

效果图: 

![icon](/images/drag_grid_overall.png)  ![icon](/images/secondary_functionalities.png)


## Animations

### Android-SpinKit

Android加载动画库

项目地址：https://github.com/ybq/Android-SpinKit

效果图：

![icon](/images/screen111.gif)


## Layout

### FlowTagLayout

Android流式布局，支持点击、单选、多选等，适合用于产品标签等，用法采用Adapter模式，和ListView、GridView用法一样

项目地址：https://github.com/hanhailong/FlowTag

效果图：

![icon](/images/flow_tag.gif)


## ImageView

### 1.PhotoView

支持双击或双指缩放的 ImageView，在 ViewPager 等 Scrolling view 中正常使用，相比上面的 AndroidTouchGallery，不仅支持 ViewPager，同时支持单个 ImageView

项目地址：https://github.com/chrisbanes/PhotoView

原理剖析文档：PhotoView

## ProgressBar

### 1.NumberProgressBar

带数字进度的进度条

项目地址：https://github.com/daimajia/NumberProgressBar

效果图：

![icon](/images/687474703a2f2f7777332e73696e61696d672e636e2f6d773639302f36313064633033346a77316566797264386e376937673230637a30326d7135662e676966.gif)

### 2.MaterialLoadingProgressBar

抽取自 SwipeRefreshLayout 的 Material Design 进度指示器

项目地址：https://github.com/lsjwzh/MaterialLoadingProgressBar

效果图：

![icon](/images/screen.gif)

### 3.CircleProgressBar

优点

1. 继承ProgressBar， 不必关心当前进度状态的保存， ProgressBar 已经在onSaveInstanceState（）和 onRestoreInstanceState(Parcelable state)中帮我们写好了。
2. 定制性很强，可以设置两种风格的进度条，设置进度条的颜色和进度文本的颜色和大小， 由于代码中对于进度文本的格化化是使用的String.format(), 所以进度文本可以根据需要随意定制
3. 代码优雅，代码注释很全面，格式整齐，可以直接在xml中设置相关的属性。
4. 
项目地址：https://github.com/dinuscxj/CircleProgressBar

效果图：

![icon](/images/CircleProgressBar.gif)

## Button

###  SwitchButton

状态切换的 Button，类似 iOS，拥有良好的用户界面

项目地址：https://github.com/kyleduo/SwitchButton

效果图：

![icon](/images/demo_140.jpg)

## Dialog

### 1.Android-AlertView

仿iOS的AlertViewController 几乎完美还原iOS 的 AlertViewController ，同时支持Alert和ActionSheet模式，每一个细节都是精雕细琢，并把api封装成懒到极致模式，一行代码就可以进行弹窗.

项目地址：https://github.com/saiwu-bigkoo/Android-AlertView

效果图：

![icon](/images/alertviewdemo.gif)

### 2.CanDialog

仿照系统Dialog所写，继承于FrameLayout，添加一些动画，一些显示类型。

项目地址：https://github.com/canyinghao/CanDialog

效果图：

![icon](/images/CanDialog.gif)



## EditText

### GridPasswordView 

模仿支付宝输入密码框

项目地址：https://github.com/Jungerr/GridPasswordView

效果图：

![icon](/images/687474703a2f2f6a756e676572722e71696e6975646e2e636f6d2f6772696470617373776f7264766965775f302e322e676966.gif)


## TextView

### 1.ATableView

ios 风格控件

项目地址：https://github.com/dmacosta/ATableView

效果图：

![icon](/images/687474703a2f2f6f6934352e74696e797069632e636f6d2f7673686e32782e6a7067.png)

### 2.android-uitableview

ios 风格控件，包括 Button、ListView、TableView

项目地址：https://github.com/Trinea/android-open-project


### SlantedTextView

一个倾斜的TextView,适用于标签效果

项目地址：https://github.com/HeZaiJin/SlantedTextView

效果图：

![icon](/images/screenshot.png)




## Time View

### 1.DateTimePicker

日期选择部件(Google Agenda 的样式风格)

项目地址：https://github.com/flavienlaurent/datetimepicker

效果图：

![icon](/images/68747470733a2f2f7261772e6769746875622e636f6d2f6269626f756e652f6461746574696d657069636b65722f6d61737465722f67726170686963732f696d67312e706e67.png)

### 2.Week View

日期控件，支持周，天视图，支持自定义样式

项目地址：https://github.com/alamkanak/Android-Week-View

效果图：

![icon](/images/screen-shot.png)

### 3.PickerView

仿 iOS 的 PickerView 控件，有时间选择和选项选择并支持一二三级联动效果，TimePopupWindow 时间选择器，支持年月日时分，年月日，时分等格式；OptionsPopupWindow 选项选择器，支持一，二，三级选项选择，并且可以设置是否联动

项目地址：https://github.com/saiwu-bigkoo/Android-PickerView

效果图：

![icon](/images/pickerdemo.gif)

## Graph View

### 1.MPAndroidChart
强大的图表绘制工具，支持折线图、面积图、散点图、时间图、柱状图、条图、饼图、气泡图、圆环图、范围（高至低）条形图、网状图等；支持图的拖拽缩放；支持 Android 2.2 以上，支持横纵轴缩放，多指缩放，展现动画、高亮、保存到 sdcard、从文件读取图表

项目地址：https://github.com/PhilJay/MPAndroidChart

效果图：

![icon](/images/68747470733a2f2f7261772e6769746875622e636f6d2f5068696c4a61792f4d50416e64726f696443686172742f6d61737465722f73637265656e73686f74732f63616e646c65737469636b63686172742e706e67.png)
![icon](/images/68747470733a2f2f7261772e6769746875622e636f6d2f5068696c4a61792f4d50416e64726f696443686172742f6d61737465722f73637265656e73686f74732f63616e646c65737469636b63686172742e706e67.png)

### 2.XCL-Charts

XCL-Charts 基于原生的 Canvas 来绘制各种图表,在设计时，尽量在保证开发效率的同时，给使用者提供足够多的定制化能力。因此使用简便,同时具有相当灵活的定制能力。目前支持 3D/非 3D 柱形图(Bar Chart)、3D/非 3D 饼图(Pie Chart)、堆积图(Stacked Bar Chart)、面积图(Area Chart)、 折线图(Line Chart)、曲线图(Spline Chart)、环形图(Dount Chart)、南丁格尔玫瑰图(Rose Chart)、仪表盘(Dial Chart)、刻度盘(Gauge Chart)、雷达图(Radar Chart)、圆形图(Circle Chart)等图表。其它特性还包括支持图表缩放、手势移动、动画显示效果、高密度柱形显示、图表分界定制线、多图表的混合显示及同数据源不同类型图表切换等。

项目地址：https://github.com/xcltapestry/XCL-Charts

### 3.android-lockpattern

Android 的图案密码解锁

项目地址：https://code.google.com/p/android-lockpattern/

Demo 地址：https://play.google.com/store/apps/details?id=group.pals.android.lib.ui.lockpattern.demo

文档介绍：https://code.google.com/p/android-lockpattern/wiki/QuickUse


## NotifyUtil

高仿淘宝，网易新闻，微信，应用宝，环聊等等热门App的通知视图，并且完通知工具类的封装，提供多达8种最常见的App通知接口,支持Android 5.0悬浮式通知样式

项目地址:https://github.com/wenmingvs/NotifyUtil

效果图：

![icon](/images/687474703a2f2f7777312e73696e61696d672e636e2f6c617267652f3639316363313531677731663037677464787935336732306263306830316c312e676966.gif)

## StepView
超炫的状态流程

项目地址：https://github.com/baoyachi/StepView

效果图：

![icon](/images/vertical_stepview.gif)


## 扁平UI

### 1.FlatUI

项目地址：https://github.com/eluleci/FlatUI

效果图：

![icon](/images/68747470733a2f2f7261772e6769746875622e636f6d2f656c756c6563692f466c617455492f6d61737465722f73616d706c652d696d616765732f73686f77636173652e706e67.png)

### 2.MaterialDesignLibrary

Material Design Android Library

项目地址：https://github.com/navasmdc/MaterialDesignLibrary



## 开发插件

### 1.[GsonFormat](https://plugins.jetbrains.com/plugin/7369?pr=androidstudio)

根据Gson库使用的要求,将JSONObject格式的String 解析成实体


### 2.[android-butterknife-zelezny](https://plugins.jetbrains.com/plugin/7369?pr=androidstudio)

配合ButterKnife实现注解，从此不用写findViewById，想着就爽啊。在Activity，Fragment，Adapter中选中布局xml的资源id自动生成butterknife注解。

### 3.[Android Parcelable code generator](https://plugins.jetbrains.com/plugin/7332?pr=androidstudio)

JavaBean序列化，快速实现Parcelable接口。

### 4.[Android Methods Count](https://plugins.jetbrains.com/plugin/8076?pr=androidstudio)

显示依赖库中得方法数

### 5.[JsonOnlineViewer](https://plugins.jetbrains.com/plugin/7838?pr=androidstudio)

在Android Studio中请求、调试接口

效果图：

![icon](/images/screenshot_15113.png)

### 6. [Android Styler](https://plugins.jetbrains.com/plugin/7972?pr=androidstudio)

根据xml自动生成style代码的插件

效果图：

![icon](/images/screenshot_15340.png)
![icon](/images/screenshot_15339.png)
![icon](/images/screenshot_15338.png)

### 7.[SelectorChapek for Android](https://plugins.jetbrains.com/plugin/7298?pr=androidstudio)

通过资源文件命名自动生成Selector文件。

效果图：

![icon](/images/screenshot_14292.png)
![icon](/images/screenshot_14291.png)
![icon](/images/screenshot_14290.png)

### 8.[gradle-retrolambda](https://github.com/evant/gradle-retrolambda)
在java 6 7中使用 lambda表达式插件

修改编译的jdk为java8:

效果图：

![icon](/images/20160311101644127)

### 9. [Material Theme UI](https://plugins.jetbrains.com/plugin/8006?pr=)

添加Material主题到你的AS

效果图：

![icon](/images/screenshot_15722.png)
![icon](/images/screenshot_15723.png)
![icon](/images/screenshot_15721.png)

### 10. [CheckStyle-IDEA](https://plugins.jetbrains.com/plugin/1065?pr=)

CheckStyle-IDEA 是一个检查代码风格的插件，比如像命名约定，Javadoc，类设计等方面进行代码规范和风格的检查，你们可以遵从像Google Oracle 的Java 代码指南 ，当然也可以按照自己的规则来设置配置文件，从而有效约束你自己更好地遵循代码编写规范。








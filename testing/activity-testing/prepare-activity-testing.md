# 建立测试环境

> 编写:[huanglizhuo](https://github.com/huanglizhuo) - 原文:<http://developer.android.com/training/activity-testing/preparing-activity-testing.html>

再开始编写,运行你的测试之前,你应该建立你的测试开发环境。本小节将会教你怎样建立Eclipse IDE来构建和运行你的测试,以及怎样用Gradle框架在命令行下构建和运行你的测试。

**注意** :为了帮助你开始,这小节是基于Eclipse及ADT插件。然而,你在自己测试开发时可以自由选用IDE或命令行。

## 用Eclipse建立测试

安装了Android Developer Tools (ADT) 插件的Eclipse将为你创建,构建,以及运行Android程序提供一个基于图形界面的集成开发环境。Eclipse的一项方便的特性是可以自动为你的Android应用项目创建一个对应的测试项目。

开始在Eclipse中创建测试环境:

1. 要是还没安装Eclipse [ADT](http://developer.android.com/sdk/installing/bundle.html)插件,请先下载安装。

2. 导入或创建你想再次测试的Android应用项目。

3. 生成一个对应于应用程序项目测试的测试项目。为你的导入项目生成一个测试项目:

>a.在项目浏览器里,右击你的应用项目,然后选择**Android Tools > New Test Project**

>b.在新建Android测试项目面板,为你的测试项目设置合适的参数,然后点击**Finish**

你现在应该可以在Eclipse环境中创建，构建和运行测试项目了。想要继续学习如何在Eclipse中进行这些任务,请转到[Creating and Running a Test Case](activity-basic-testing.html)

## 用命令行建立测试

如果正在使用Gradle version 1.6或者更高的版本作为构建环境,可以用Gradle Wrapper创建。构建和运行Android应用测试。确保你的gradle.build文件中默认[minSdkVersion](http://developer.android.com/guide/topics/manifest/uses-sdk-element.html)属性是8或更高。可以参考包含在这下载包中的示例文件gradle.build

用Gradle Wrapper运行你的测试:

1. 连接你的Android真机或开启你的Android模拟器。

2. 在你的项目目录运行如下命令:

>./gradlew build connectedCheck

进一步学习Gradle关于Android测试的内容,参看[Gradle Plugin User Guide](http://www.gradle.org/docs/current/userguide/userguide_single.html)。

进一步学习使用Gradle及其它命令行工具,参看[Testing from Other IDEs.](http://developer.android.com/tools/testing/testing_otheride.html)。

本节示例代码[AndroidTestingFun.zip](http://developer.android.com/shareables/training/AndroidTestingFun.zip)

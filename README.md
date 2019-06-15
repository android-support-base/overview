# android-support-base
* Android Component SDK(功能组件)

## 特性(feature)
* 基于Android APIs and Google APIs
* 不依赖第三方类库
* 组件，功能导向

## 效用(utility)
* 基类，抽象，接口
* 可复用(Reuseable)，快速开发，不涉及具体的业务

## 类库

### Stable Library - Java
| Branch | Description |
| ------------- | ------------- |
| [android-support-log](https://github.com/android-support-base/log) | 日志库 |
| [android-support-utils](https://github.com/android-support-base/utils) | 工具库，解决兼容性问题 |
| [android-support-ui](https://github.com/android-support-base/ui) | 轻量级界面库 |
| [android-support-net](https://github.com/android-support-base/net) | 网络库，简单的网络请求库 |
| [android-support-io](https://github.com/android-support-base/io) | 数据处理库 |

### Dev Library - Java
| Branch | Description |
| ------------- | ------------- |
| [android-support-image](https://github.com/android-support-base/image) | 图片库 |
| [android-support-download](https://github.com/android-support-base/download) | 简易的下载类库 |
| [android-support-video](https://github.com/android-support-base/video) | 简易的下载类库 |
| [android-support-web](https://github.com/android-support-base/web) | 网页库，解决兼容性问题 |

### Dev Library - Kotlin
* none

### 使用
- 方式一：依赖jcenter发布版本
```
dependencies{
    implementation 'com.amlzq.android:xxx:latest.integration'
}
```
- 方式二：编译项目，并打包到本地maven库
```
local.properties文件中配置：

# Local maven
mavenLocal=file://C://Users/用户名/.m2/repository/

执行 gradlew uploadArchives

dependencies{
    implementation 'com.amlzq.android:xxx:latest.integration'
}
```

## 规划
* 借鉴[android.support.v4](https://developer.android.com/topic/libraries/support-library/features.html#v4-compat)拆分思路
```
v4 compat 兼容库
v4 core-utils 工具库
v4 core-ui 用户界面库
v4 media-compat 媒体兼容库
v4 fragment 碎片库
```

## 最后
* base split to each branch by 2018-05-26
* common rename into base by 2018-05-01
* sample rename into common by 2017-08-01
* June 13, 2016 at Mingzhu Garden
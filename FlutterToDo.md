# FlutterToDo



## 安装

[Windows install - Flutter](https://flutter.dev/docs/get-started/install/windows)

解压后放在 `C:\src\flutter` 中

环境变量 `C:\src\flutter\bin`

查看是否缺必要依赖`C:\src\flutter>`

```sh
flutter doctor
```

同意证书

```
flutter doctor --android-licenses
```

如果安装的慢，需要换源，上交大源。https://flutter.dev/community/china

就是添加两个Path：

````
FLUTTER_STORAGE_BASE_URL: https://mirrors.sjtug.sjtu.edu.cn/
PUB_HOSTED_URL: https://dart-pub.mirrors.sjtug.sjtu.edu.cn/
````

## IDE

安装 Android Studio，安装 Flutter 插件。需要代理

安装 VS code ，安装 Flutter 插件。

连接手机，开发者模式，usb debug 模式



## 修改Android SDK版本

在 `android\app\build.gradle` 修改 `compileSdkVersion 30` `targetSdkVersion 30`

## 设置gradle源

为阿里云

在 `android\build.gradle` 修改两处

在 `C:/src/flutter/packages/flutter_tools/gradle/flutter.gradle` 修改一处

````
    repositories {
        //google()
        //jcenter()
        maven { url 'https://maven.aliyun.com/repository/google' }
        maven { url 'https://maven.aliyun.com/repository/jcenter' }
        maven { url 'http://maven.aliyun.com/nexus/content/groups/public' }

    }
````


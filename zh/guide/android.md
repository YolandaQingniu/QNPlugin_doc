# Android 快速集成 

## Android Studio

### Android 使用gradle集成
* 在你工程的根目录下的 **build.gradle**添加**jitpack**支持
```
    allprojects {
		repositories {
			//其它仓库配置
			maven { url 'https://jitpack.io' }
    }
}
```
* 在你的module的根目录下的**build.gradle**添加依赖[最新版本查看地址](https://github.com/YolandaQingniu/qnscalesdkX/releases/)

```
<!--这里的版本号，x.x.x 可以指定为任意release版本-->
<!--如果希望一直使用最新版本可以替换 x.x.x 为 master-SNAPSHOT -->

dependencies {
        ...
        compile 'com.github.YolandaQingniu:qnscalesdkX:x.x.x'
}
```
### 本地依赖


* 下载最新的[jar和so库](https://github.com/YolandaQingniu/qnscalesdkX/releases/)，导入下载的.zip压缩包中的`jar和so库`
* 在清单文件中申请蓝牙权限、位置权限、网络权限（离线SDK不需要）

    ```
    xml
   <!--蓝牙权限-->
   <uses-permission android:name="android.permission.BLUETOOTH" />
   <uses-permission android:name="android.permission.BLUETOOTH_ADMIN" />
   <!--6.0及之后需要动态申请-->
   <uses-permission android:name="android.permission.ACCESS_COARSE_LOCATION" />
   <uses-permission android:name="android.permission.ACCESS_FINE_LOCATION" />
   <!--用来存储日志-->
   <uses-permission android:name="android.permission.READ_EXTERNAL_STORAGE" />
   <uses-permission android:name="android.permission.WRITE_EXTERNAL_STORAGE" />
   <!--如果是在线的sdk需要网络权限-->
   <uses-permission android:name="android.permission.INTERNET" />
   <!--qnscalesdk:1.1.3-beta3 之前(包含1.1.3-beta3)的版本需要增加此权限，之后的版本不需要-->
  <uses-permission android:name="android.permission.FOREGROUND_SERVICE" />
  <!--qnscalesdk:1.1.3-beta3 之后(1.1.3-beta4开始)的版本需要增加此权限，之前的版本不需要-->
   <uses-permission android:name="android.permission.WAKE_LOCK" />   
    ```

* 需要在**AndroidManifest.xml**注册SDK中的组件：

```
xml
 <!--qnscalesdk:1.1.3-beta3之前(包含1.1.3-beta3)的版本配置-->
<service android:name="com.qingniu.qnble.scanner.BleScanService"/>
<service android:name="com.qingniu.scale.measure.ble.ScaleBleService"/>
<service android:name="com.qingniu.scale.measure.broadcast.ScaleBroadcastService"/>
<service android:name=".measure.broadcast.ScaleFoodBroadcastService" />


<!--qnscalesdk:1.1.3-beta3 之后(1.1.3-beta4开始)的版本配置-->
<service android:name="com.qingniu.qnble.scanner.BleScanService" android:permission="android.permission.BIND_JOB_SERVICE"/>
<service android:name="com.qingniu.scale.measure.ble.ScaleBleService" android:permission="android.permission.BIND_JOB_SERVICE"/>
<service android:name="com.qingniu.scale.measure.broadcast.ScaleBroadcastService" android:permission="android.permission.BIND_JOB_SERVICE"/>
<service android:name="com.qingniu.scale.wsp.ble.ScaleWspBleService" android:permission="android.permission.BIND_JOB_SERVICE" />
<service android:name="com.qingniu.scale.measure.broadcast.ScaleFoodBroadcastService" android:permission="android.permission.BIND_JOB_SERVICE" />
<service android:name=".measure.broadcast.ScaleFoodBroadcastService" android:permission="android.permission.BIND_JOB_SERVICE" />
<service android:name="com.qingniu.heightscale.ble.HeightScaleBleService" android:permission="android.permission.BIND_JOB_SERVICE" />
 ```   
* SDK中使用到了v4包的资源，开发者项目中需要引入v4包的资源

## 混淆配置(proguard-rules)
```
-keep class com.qingniu.scale.model.BleScaleData{*;}
```
## 其它

配置文件的集成方式可以参考demo。放在`assets`目录，然后在初始化时使用："file:///android_asset/文件名.qn"来传文件路径


# iOS 快速集成 

SDK的运行需要appid以及配置文件，商家在接入时可先使用Yolanda提供的测试appid和测试配置文件，正式发布时必须向Yolanda官方获取正式appid和配置文件

## 安装方式

### cocoapods安装:
- 先安装Cocoapods；
- 通过 pod repo update 更新QNSDK的cocoapods版本；
- 在Podfile对应的target中，添加`pod 'QNSDK'`，并执行pod install；
- 在项目中使用CocoaPods生成的.xcworkspace运行工程；
- 在你的代码文件头引入头文件`#import <QNSDK/QNDeviceSDK.h>`

### Carthage安装:
- 安装 Carthage；
- 打开 Cartfile, 添加 `github "https://github.com/YolandaQingniu/sdk-ios-demo.git"`；
- 打开命令行, cd 到你的 project 目录, 输入 carthage update；
- 将 Carthage/Build/ 目录下的 `QNSDK.framework` 拖到你的项目工程配置的 Build Phases -> Linked Binary and Libraries 里面；
- 在你的代码文件头引入头文件`#import <QNSDK/QNDeviceSDK.h>`

### 手动安装:
- 下载SDK安装包至工程
- 引入SDK路径 【TARGETS】-> 【Build Setting】->【Search Paths】->【LibrarySearch Paths】中添加SDK路径
- 配置链接器 【TARGETS】-> 【Build Setting】-> 【Linking】-> 【Other Linker Flags】中添加 `-ObjC`、`-all_load`、`-force_load [SDK路径]` 其中之一

## 工程的配置

- 在Info.plist中有对 【Privacy - Bluetooth Peripheral Usage Description】【Privacy - Bluetooth Always Usage Description】 键 进行蓝牙的使用说明

## 注意事项
- SDK适配8.0及以上系统
- iOS10.0及以上系统必须Info.plist中配置蓝牙的使用说明，否则无法使用系统的蓝牙功能
- iOS13.0及以上系统必须Info.plist中配置蓝牙的使用授权说明，否则会发现奔溃
- 必须为SDK配置链接器，否则SDK无法正常运行

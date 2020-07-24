# WKCCoolCameraView
自定义相机

[![Carthage compatible](https://img.shields.io/badge/Carthage-compatible-4BC51D.svg?style=flat)](https://github.com/Carthage/Carthage#adding-frameworks-to-an-application) [![CocoaPods compatible](https://img.shields.io/cocoapods/v/WKCCoolCameraView?style=flat)](https://cocoapods.org/pods/WKCCoolCameraView) [![License: MIT](https://img.shields.io/cocoapods/l/WKCCoolCameraView?style=flat)](http://opensource.org/licenses/MIT)

只有相机的基础界面， 其他都可高度自定义.
使用: 拖进工程或 `pod WKCCoolCameraView`

# 属性列表
| 属性 | 含义 |
| ---- | ---- |
| mode | 模式(拍照or录像) |
| position | 摄像头位置 |
| isFront | 是否前置 |
| isCapturing | 是否正在捕捉画面 | 
| shouldTapFocus | 是否能点击聚焦| 
| shouldPinchZoomEnable | 是否支持捏合缩放 |
| maxZoomScale | 捏合缩放最大比例|
| focusPoint | 聚焦点 | 
| exposurePoint | 曝光点 |
| flashMode | 闪光灯模式|

# 方法列表
开始捕捉 ` startCapture() `
停止捕捉 ` stopCapture() `
开始录像 ` startVideoRecord(filePath = nil) `
停止录像 ` stopVideoRecord() `
销毁存储的录像 ` inviladeVideoRecord() `
切换摄像头 ` switchCamera() `
切换闪光灯 ` switchFalsh() `
拍照 ` takePhoto() `
设置曝光值 `setExposure(value = 0) `
重置相机坐标 ` resetFrame(frame = .zero)`

# 代理回调
流回调 ` coolCameraDidOutputVideoBuffer(cool: WKCCoolCameraView, sampleBuffer: CMSampleBuffer) `
拍照 ` coolCameraDidTakePhoto(cool: WKCCoolCameraView, image: UIImage) `
录像 ` coolCameraDidVideoRecorded(cool: WKCCoolCameraView, videoPath: String) `
点击聚焦 ` coolCameraDidFocus(cool: WKCCoolCameraView, point: CGPoint) `
捏合缩放 ` coolCameraDidZoom(cool: WKCCoolCameraView, zoom: CGFloat) `

[OC](https://github.com/WKCLoveYang/WKCFansyCameraView)

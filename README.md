# ChromaticFocus

[![Build macOS app](https://github.com/cccccxh1023/ChromaticFocus/actions/workflows/build.yml/badge.svg)](https://github.com/cccccxh1023/ChromaticFocus/actions/workflows/build.yml)

一个实验性的 macOS 菜单栏显示滤镜：红通道保持清晰，绿通道轻度圆盘模糊，蓝通道使用更大的圆盘模糊，并按照显示器物理尺寸、原生像素和用户输入的观看距离换算滤镜半径。

> ChromaticFocus 不是经过验证的近视治疗，也不代表能够永久缩短眼轴。当前版本是供测试使用的 beta 版。

## 直接下载 App

**[下载 ChromaticFocus-macOS.zip](https://github.com/cccccxh1023/ChromaticFocus/releases/download/v0.1.2-beta/ChromaticFocus-macOS.zip)**

不需要安装 Xcode，不需要打开终端，也不需要自己编译。

系统要求：macOS 13 或更高版本；同时支持 Apple 芯片和 Intel Mac。

## 安装

1. 下载并解压 `ChromaticFocus-macOS.zip`。
2. 把 `ChromaticFocus.app` 拖入“应用程序”。
3. 第一次请右键 `ChromaticFocus.app`，选择“打开”。
4. 如果 macOS 仍然拦截，请进入“系统设置 → 隐私与安全性”，在页面下方选择“仍要打开”。
5. 允许“屏幕与系统音频录制”权限；授权后可能需要退出并重新打开 App。

ChromaticFocus 是菜单栏 App，不会出现在 Dock。启动后请在屏幕右上角寻找眼睛图标。

## 基本使用

1. 选择需要处理的显示器。
2. 输入眼睛到屏幕的大致距离。
3. 建议先从 `Adaptation · 50%` 开始。
4. 点击启用滤镜。

紧急关闭快捷键：`Control–Option–Command–R`（`⌃⌥⌘R`）。

## 自动调节

程序会自动读取显示器的原生像素、Retina 缩放、物理尺寸和旋转状态，并在显示器发生变化时重新计算。电脑无法自动知道眼睛到屏幕的实际距离，因此观看距离需要由用户输入一次。外接显示器报告的物理尺寸异常时，可以手动填写显示器宽度。

## 隐私

- 不捕获音频；
- 不保存截图或录屏；
- 不上传屏幕画面；
- 不包含分析、广告或第三方跟踪；
- 屏幕帧只在本机内存和 GPU 中实时处理。

## 当前状态

这是 `0.1.2 beta`。GitHub Actions 已通过几何计算测试，并成功编译、临时签名和打包了通用 macOS App。由于没有 Apple Developer ID，当前 App 尚未经过 Apple 公证，第一次开启通常需要使用右键“打开”。

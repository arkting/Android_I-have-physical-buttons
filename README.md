# I have physical buttons! (我有物理按键！)

[English](#english) | [中文](#中文)

---

<div id="english"></div>

## English

**I have physical buttons!**

On stock-like Android systems, the gesture pill (navigation bar) has always been a headache. With every Android update, various modules often fail to keep up with Google's pace, making the hiding process unstable.

This is a wonderful discovery: when Android believes the phone has physical buttons, the navigation bar naturally disappears. Surprisingly, this hidden navigation bar does not cause gesture navigation to fail; all functions remain perfectly normal. Only the gesture pill vanishes—no placeholders, no black bars—though the functional buttons below the keyboard will also disappear.

Theoretically, regardless of the Android version, we only need to inject `qemu.hw.mainkeys=1` into `system.prop` to achieve this effect. Yes, just one line.

However, because Android identifies physical buttons, if you are currently using three-button navigation (or other navigation methods), you will lose your navigation buttons. Gesture navigation, however, will not be affected.

**Note:** If your ROM has deeply customized navigation logic, this method will likely not work.

But if you intend to use third-party gesture software, this might be exactly what you need. Simply set your system to three-button navigation and enable this module, and no system navigation will interfere with your custom gestures.

If you are capable, you can directly modify `system.prop` instead of installing a module. If you prefer using a module, please download it from the **Releases** section.

This module has only been tested on Pixel phones, including the latest Android 16 factory images and universal GSIs. It works perfectly on these systems, but has not been tested on other ROMs.

This module likely won't need an update for several years (which is why I boldly stated "Applies to all Android versions"). It is not guaranteed to work on all Android devices; if it does not work on yours, please remove it.

---

<div id="中文"></div>

## 中文

**我有物理按键！**

在类原生系统上，小白条（导航栏）一直是个令人头疼的问题。随着 Android 的更新，各个模块往往跟随不上 Google 的进度，隐藏效果开始变得不稳定。

这是一个奇妙的发现：当 Android 认为手机存在实体按键时，导航理应会消失。但意外的是，消失的导航栏并不会导致手势失效，所有功能完全正常。仅仅是小白条消失了，没有占位，没有黑边，只不过键盘下方的功能按键（如下降箭头等）也会消失。

所以理论上，不管 Android 版本如何，我们只需要在 `system.prop` 中注入 `qemu.hw.mainkeys=1`，就能实现这样的效果。没错，一行即可。

但是，由于 Android 识别到了物理按键，所以如果你正在使用三键导航（或者其他导航方式），那你将会失去导航按钮。但手势操作是不会受到影响的。

**注意：** 如果你的 ROM 深度定制了导航逻辑，那么该方法大概率不再适用。

但如果你想使用第三方手势软件，那这可能正如你所愿：你只需要设置为三键导航再启用模块，就不会存在任何系统导航来干扰你的自定义手势了。

如果你有能力，完全可以直接修改 `system.prop` 而无需安装模块。如果你需要使用模块，请从 **Releases** 中下载。

该模块只在 Pixel 手机上测试过，包含了最新的 Android 16 原厂镜像和通用 GSI，在这些系统上运行完美，但其他 ROM 则未有过测试。

该模块大概率在未来几年内都不需要更新（所以我大胆地写下了适用于所有 Android 版本）。由于不保证适用于所有 Android 设备，如果它在你的设备上不工作，请移除该模块。

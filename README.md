# I have physical buttons!

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

<h1 align="center">"Challenging the Strongest HyperOS iOS Emulation on the Entire Site — True Pixel-Level Restoration"</h1>

<p align="center">
  <img src="./images/cover.jpg" width="90%">
</p>

# Preface

> [!IMPORTANT]
>  This illustrated guide's testing, comparison, and production took two months in total. I have selected and aggregated the iOS-emulation modules I believe currently imitate iOS most closely, making this a high-quality update.
>
> Once again: this guide only aims to achieve the best possible emulation effect while using fewer modules. To achieve the emulation effect, some places may include beautifications unsuitable for daily use — please decide for yourself what to keep.

```
• Test device: Xiaomi 12X
• Resolution: 2400 x 1080
• System version: OS 1.0.3.0.UMACNXM By S.Team ColdCat | Android 14
• ROOT manager: Kitsune Mask_26.4-kitsune-2
• Theme & Wallpaper version: 4.2.2.6 (Official)
```

> [!NOTE]
> Note: The specific parameters for the settings below are all based on the environment above; please adjust according to your actual situation.

> [!TIP]
> All files are available in the link at the end of the document; links in the guide are only references to sources.
>
> For all settings in the modules not mentioned or not screenshotted in this guide, keep them at default.

# 🌸🌸🌸The tutorial starts now🌸🌸🌸

## 🔴 Table of Contents & Preview
### ⭕ Table of Contents

* [1. Theme](#🔴-一主题)
* [2. Lock Screen](#🔴-二锁屏)
* [3. Home Screen](#🔴-三桌面)
* [4. Status Bar](#🔴-四状态栏)
* [5. Notification Center](#🔴-五通知中心)
* [6. Control Center](#🔴-六控制中心)
* [7. Others](#🔴-七其他)
* [8. Advanced](#🔴-八进阶)

### ⭕ Preview
- I will introduce them one by one from the outside in, following the order of the table of contents.
- 📱 Finished product demo

  <img src="./images/iOS_Demo_Watermark.gif" width="30%">

## 🔴 1. Theme

### ⭕ 1. Theme Crack
- Version: 1.8.0-for 0.07
- Source: The original developer has stopped updating; obtained from the "Theme Crack" section.

### ⭕ 2. Theme
- Theme: `学长iOS17 HyperOS (Official System Component Version)`
- Source: https://www.coolapk.com/feed/51457930
- Note: Respect the original author; please obtain it from the original author's backend. The version number and checksum I used are in the shared files. Hereinafter referred to as `"学长iOS17"`.

### ⭕ 3. Font
- Font: 学长iOS16 PingFang
- Note: Built into the `"学长iOS17"` theme.

### ⭕ 4. Core Crack
- Software: `HyperCeiler` (version and source omitted hereinafter)
- Version: 2.3.135_20231231(135)_beta
- Source: Official Beta Test channel
- Settings: `⚙️System Framework→Package Management Service: [Enable all first five items]`

## 🔴 2. Lock Screen

- Theme: `"学长iOS17"`
- Wallpaper: My wallpaper files are shared in the link at the end of the document.
- Note: Because HyperOS still has issues when directly applying lock screen wallpapers under third-party themes, you need to first import the wallpaper into the theme's mtz file, replace the original lock screen wallpaper, and then apply the modified theme.
- Settings:

  <img src="./images/2.jpg" width="50%">

- Settings [Optional]:
`⚙️System Settings→Notifications & Status Bar→Status Bar - Pull-down while locked→Control Center: [Enable]`

## 🔴 3. Home Screen

### ⭕ 1. Wallpaper
- Wallpaper: Already imported into the mtz file in `2. Lock Screen`.

### ⭕ 2. Icons

#### ① Basic Icons
- Theme: `"学长iOS17"`

#### ② Extra Icons
- Software: `创建快捷方式_1.17` (Create Shortcut)
- Description: Can create custom-styled icons on the home screen. The app is not hard to use; steps omitted.

### ⭕ 3. Stacked Home Screen
- Software: `HyperOS堆叠桌面2.2.7.1(文件夹名称居中)` (HyperOS Stacked Desktop 2.2.7.1, folder name centered)
- Source: https://www.coolapk.com/feed/53758297
- Note: Install using Core Crack (HyperCeiler). This is the first version that "fixes the issue of blur loss when switching themes"; tested and can be kept long-term.
- Description: My shared file has "folder title centered" modified; see my post for the specific modification process: https://www.coolapk.com/feed/53836371. If you find it useful, please give the original author a quality coin at the post above.
- Settings:

  <img src="./images/3-3.jpg" width="50%">

### ⭕ 4. Home Screen Widgets
- Software: `KWGT (Pro)`; `OS小组件内测_0.1.0` (OS Widgets Beta 0.1.0)
- Source: LITEAPKS; shared by 学长
- Note: Remember to enable autostart for the software and set the battery saver policy to unrestricted.
- KWGT settings (2x2 & 4x2):
  ```
  ⚙️Root directory→Layer-Scale: [107]
  ⚙️Root directory→Item-OS Widget→Position-Y Offset: [0]
  ⚙️For specific data in the widget (e.g., weather region), adjust in "Root directory→Global Variables".
  ⚙️To edit the widget a second time, tap the widget name on the home screen.
  ```
- Steps:

  <img src="./images/3-4.jpg" width="50%">

### ⭕ 5. Dock & Layout
- Software: `HyperCeiler`
- Settings:

  <img src="./images/3-5.jpg" width="50%">

### ⭕ 6. Gesture Bar & Volume Slider
- Software: `MIUI Extra`
- Version: 2.6.9.2-U-Pre_Hyper
- Source: Github
- Settings:

  <img src="./images/3-6.jpg" width="50%">

### ⭕ 7. Negative One Screen (App Vault)
- Software: `智能助理(魔改版)` (Smart Assistant, modded); `HyperCeiler`; `KWGT (Pro)`; `OS小组件内测_0.1.0`
- Source: Coolapk @想吸猫的狗; the original post is no longer viewable.
- Note: The Smart Assistant's version number has been changed to prevent restoration on reboot; install using Core Crack (HyperCeiler).
- KWGT settings:
  ```
  ⚙️Root directory→Layer-Scale: [102] (4x2) & [104] (2x2)
  ⚙️Root directory→Item-OS Widget→Position-Y Offset: [18]
  ⚙️Since the name of the App Vault widget is outside the frame and cannot be tapped, to edit the App Vault widget a second time, first tap any widget name on the home screen, then go through the top-left "≡"→"Available Space" and select it for editing.
  ```
- Settings:

  <img src="./images/3-7.jpg" width="50%">

### ⭕ 8. Page Indicator to Search Box
- ⌾Description: Regarding the search box, @懶貓雜貨鋪 made a very detailed video tutorial: https://www.coolapk.com/feed/54067260. However, since my tutorial involves wallpaper zoom animation, sticking the search directly on the wallpaper would make the recents animation look rather messy. So this is only included here for reference; I personally won't use it daily — those who need it can try.

## 🔴 4. Status Bar
Theme: `"学长iOS17"`

### ⭕ 1. Dynamic Island
- Software: `dynamicSpot_1.52 (Chinese Pro version)`
- Source: Shared by 学长
- Settings:

  <img src="./images/4-1.jpg" width="50%">

- Note 1: Remember to enable autostart for the software and set the battery saver policy to unrestricted.
- Note 2: This software has newer versions, but the new versions have issues with permanent display, so just use this version.

### ⭕ 2. Disable Dynamic Forehead
- Software: `HyperCeiler`
- Settings: See bottom-right of `Figure 4-1`.

### ⭕ 3. Disable System Popups
- Software: `popupControl (Chinese Pro version)`
- Source: https://www.coolapk.com/feed/52215824
- Settings: See `Figure 4-1`.
- Note: Remember to enable autostart for the software and set the battery saver policy to unrestricted.

### ⭕ 4. Status Bar Adjustment

#### ① Necessary System Settings
- Settings: See bottom-left of `Figure 4-4`.

#### ② Icon Position Fine-tuning
- Software: `米客` (MiKe) (version and source omitted hereinafter)
- Version: 24.01.24
- Source: Github
- Settings: See `Figure 4-4`.
- Description: This item mainly tries to control the Dynamic Island so that when activated, it exactly covers one complete icon on each side — in other words, whether the Dynamic Island is active or not, try to avoid icons being cut off by the Dynamic Island's edge, making the animation less abrupt. At the same time, move the clock position slightly to the right, and place the Do Not Disturb icon to its right, further imitating iOS. (See top-right of `Figure 4-4`)
- Screenshot:

  <img src="./images/4-4.jpg" width="50%">

### ⭕ 5. Dual-row Mobile Network Icons [Optional]
- Description: If you are a dual-SIM user, you can try this step.
- Software: `米客`
- Settings: See top-left of Figure 4-4.

## 🔴 5. Notification Center
⚠️Note: Currently no emulation module specifically for the Notification Center has been found; we can only borrow 米客 to imitate the iOS style as much as possible.
- Software: `米客`
- Settings:

  <img src="./images/5.jpg" width="50%">

## 🔴 6. Control Center

### ⭕ 1. Basics
- Software: `系统界面组件` (System UI Components)
- Source: Self-modified https://www.coolapk.com/feed/53817553
- Note: Install using Core Crack (HyperCeiler).
- Aside: This version is indeed already good, but not the final solution; I will further optimize it. Those interested can follow my posts for the latest news on my second modification.

### ⭕ 2. Details
- Software: `米客`
- Settings:

  <img src="./images/6.jpg" width="50%">

- Description: You can copy the Apple character here: []. If your font is set correctly in `1.3`, this icon can display normally.

## 🔴 7. Others
⚠️Note: This section contains some scattered small details of iOS emulation.

### ⭕ 1. Global Sound Effects
- Module: `A-这小子做了个iOS提示音（iOS 17 版）！` (A — This guy made an iOS notification sound (iOS 17 version)!)
- Source: https://www.coolapk.com/feed/49413867
- Note: Flash in Magisk; before flashing, please disable Shamiko (if present). After rebooting, in System Settings → Sound & Touch, set the first three sound items to `水滴` (Water Drop), `小米清新版` (Xiaomi Fresh), and `白日梦` (Daydream) respectively; for the rest (lock screen, screenshot, etc.), test on your own whether they applied successfully.

### ⭕ 2. iOS Volume Slider
- Software: `Volume Style (Pro)`
- Source: ddooo
- Settings:

  <img src="./images/7-2.jpg" width="50%">

### ⭕ 3. iOS Keyboard
- Software: `BM iOS Keyboard_2023`
- Source: BMModS
- Description: The English part of this input method is fairly complete, but it doesn't support Chinese. So it can only be used for demonstration during emulation, and is not yet suitable for daily use.
- Note: You can turn on the keyboard key sound effects for fun; the simulation is decent.

## 🔴 8. Advanced
⚠️Note: This section includes the parts involving code modification in the iOS emulation process. Beginners only need to know that opening the theme with MT Manager and opening the files named after package names inside as archives is entirely sufficient for this chapter's modifications.

### ⭕ 1. Fix the volume slider sinking issue in landscape mode of the theme.
- File location: `./miui.systemui.plugin/theme_values.xml`
- Delete the lines containing the following variables:
  - Line 16: `miui_volume_column_height`
  - Line 20: `miui_volume_column_width`
  - Line 36: `miui_volume_offset_top_collapsed`
- Same for the `nightmode` folder.

### ⭕ 2. Solve the issue of folder title misalignment after reboot under the second-modified home screen of the theme.
- File location: `./com.miui.home/theme_values.xml`
- Resource name: `folder_edit_text_margin_left`
- Modified value: `0dp`
- Same for the `nightmode` folder.

# 🌸🌸🌸The tutorial ends here🌸🌸🌸

## ⭕ Download Link `Choose one`

- Download this repository directly

  <a href="https://github.com/MrBocchi/HyperiOS/archive/refs/heads/main.zip"><img src="./images/Repository.png" alt="Repository Link" width="50%"></a>

- 123 Cloud Drive `Extraction code: 6666`

  <a href="https://www.123pan.com/s/Kb4vjv-5ooJh.html"><img src="./images/123pan.png" alt="123 Pan Link" width="50%"></a>

---
> [!WARNING]
> Unauthorized reproduction prohibited; for derivative works, please credit the source.
>
> Topics: #HyperOS# #iOS Emulation Theme# #MIUI Theme#

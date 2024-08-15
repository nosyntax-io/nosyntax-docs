---
slug: /visual_assets
title: Visual Assets
description: Visual Assets
tags: [Launcher Icon]
sidebar_position: 0
keywords: [NoSyntax, Launcher Icon]
---

# Visual Assets

Visual assets are key to defining your app’s visual identity and establishing its brand. These assets—including the app icon, launcher icon, and splash icon—are crucial for creating a cohesive and professional appearance.

## Launcher Icon

The launcher icon is the first visual element users see when installing your app. It is crucial for making a strong first impression and plays a key role in your app’s branding. A well-designed launcher icon helps your app stand out on users' devices and ensures a professional appearance.

### Adding Launcher Icon

To add your launcher icon, follow these steps:

1. Navigate to **General** > **Visual Assets**.

2. In the **Launcher Icon** section, click **Upload** and select your icon file.

3. Rebuild the app to apply the changes.

:::tip

For better results, ensure your launcher icon is at least **512x512 pixels**, in **PNG** or **JPEG** format, and has no padding.

:::

### Manually Adding Launcher Icon for Android

If you’re using the foundation template and need to add a launcher icon in **Android Studio**, follow these steps:

1. **Open Android Studio**: Launch the project in Android Studio.

2. **Open Image Asset Studio**:
    - Right-click the `res` folder in the **Project** window.
    - Select **New** > **Image Asset**.

3. **Configure Icon**:
    - Set **Icon Type** to **Launcher Icons (Adaptive and Legacy)**.
    - Under the **Foreground Layer**, choose the icon file and adjust scaling and padding as needed.
    - Optionally, modify the **Background Layer** settings as needed.

4. **Generate Icons**:
    - Click **Next**, then **Finish** to generate the icons in the `mipmap` folders.

5. **Rebuild Project**: Rebuild the project to apply the new launcher icon.

<div class="video-container"><iframe src="https://www.loom.com/embed/f4cb4ccaac2c400c968a4b43f0b60a33?sid=8217e5f6-abde-469d-b9aa-d76c04149b3d" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe></div>

## Splash Icon

The splash icon is the first visual element users see when opening your app. It sets the tone and creates a strong first impression. A well-designed splash icon enhances your brand and ensures a polished, professional look.

### Adding Splash Icon

To add your splash icon, follow these steps:

1. Navigate to **General** > **Visual Assets**.

2. In the **Splash Icon** section, click **Upload** and select your icon file.

3. Rebuild the app to apply the changes.

:::tip

For Android, we use the [**Splash Screen API**](https://developer.android.com/develop/ui/views/launch/splash-screen) to adhere to best practices. Although most splash screen setup is handled automatically, the quality of your splash screen depends on the icon you upload. Please ensure your splash icon meets these criteria:

- Ensure your splash icon is at least **512x512 pixels**.
- Use **JPEG** or **PNG** format.
- Avoid adding padding (this will be adjusted during the build process).

:::

### Manually Adding Splash Icon for Android

If you’re using the foundation template and need to add a splash icon, follow these steps:

1. Place your splash icon file in the `app/src/main/res/drawable/` directory.

2. Rebuild the app to apply the changes.

:::tip

For best results, refer to the [**Splash Screen API**](https://developer.android.com/develop/ui/views/launch/splash-screen) documentation for comprehensive guidelines.

:::
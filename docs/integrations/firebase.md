---
slug: /integrations/firebase
title: Firebase
description: Firebase
tags: [Firebase, Integration, Analytics, Crash Reporting]
sidebar_position: 0
keywords: [NoSyntax, Firebase, Integration, Analytics, Crash Reporting]
---

# Firebase

Integrating Firebase with your application unlocks powerful features such as push notifications,
analytics, crash reporting, and more. These tools allow you to engage users effectively, monitor app
performance, and maintain stability, enhancing the overall user experience.

## Firebase Setup

To integrate Firebase with your app, you first need to create and configure a Firebase project. Follow the steps below to set up your Firebase project.

### Create a Firebase Project

Follow these steps to create a Firebase project:

1. Go to [Firebase Console](https://console.firebase.google.com/) and sign in with your Google account.

2. Click **Get started with a Firebase project**.

3. Follow the prompts to name your project and set up the necessary configurations.

4. Click **Create a Project** to complete the setup.

For a detailed step-by-step guide, watch the walkthrough video below.

<div class="video-container"><iframe src="https://www.youtube.com/embed/NJMW2app0VI?si=m6R2P98M5j_Ca04d" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe></div>

### Add Firebase to Your Android App

After creating your Firebase project, follow these steps to add your app to Firebase:

1. On the project overview page, click the **Android Icon**.

2. Enter your app's package name and nickname, then click **Register App**.

3. Click **Download google-services.json** to download your config file. Keep it secure as you'll need it later.

4. Skip the Firebase SDK integration step, as it has already been set up.

:::warning[Please note]

Ensure the package name matches the one used in your app's configuration; otherwise, it won't work. You can find the package name in NoSyntax under **General Settings** > **App Details** > **App ID**.

:::

For a detailed step-by-step guide, watch the walkthrough video below.

<div class="video-container"><iframe src="https://www.youtube.com/embed/NJMW2app0VI?si=m6R2P98M5j_Ca04d" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe></div>

## Enable Firebase in NoSyntax

To enable Firebase in NoSyntax after setting up your Firebase project, follow these steps:

1. Navigate to **Settings** > **Integrations** > **Firebase**.

2. Upload the Firebase config file you downloaded.

3. Rebuild your app to apply the changes.

## Manual Integration

If you've downloaded the foundation template, which comes as a basic setup without pre-configurations, you can manually set up Firebase. The necessary dependencies and code are already included.

### Android Setup Instructions

To manually configure Firebase for Android, follow these steps:

1. Place the config file into the **module (app-level)** root directory of your project.

2. Rebuild the project to apply the changes.

:::warning[Please note]

Ensure the package name in your app's **app-config.yml** file matches the one in your Firebase project. A mismatch will cause the build to fail with the error: **"No matching client found for package name: [package name]"**.

:::
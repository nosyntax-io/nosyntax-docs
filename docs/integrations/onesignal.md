---
slug: /integrations/onesignal
title: OneSignal
description: OneSignal
tags: [OneSignal]
sidebar_position: 0
keywords: [OneSignal]
---

# OneSignal

Integrating OneSignal with your application provides advanced push notification features such as targeted messaging, in-app messaging, and user segmentation. These features boost user engagement and improve the overall experience by delivering personalized and timely notifications.

:::note[Prerequisites]
  OneSignal relies on Firebase to function. To integrate OneSignal with your app, start by creating and configuring a Firebase project. For detailed instructions, refer to the [**Firebase Setup**](https://docs.nosyntax.io/integrations/firebase) guide. 
:::

## OneSignal Setup

To integrate OneSignal with your app, you need to create and configure a OneSignal app. This section will guide you through the setup process.

### Creating a OneSignal App

Follow these steps to create a OneSignal app:

**Step 1: Create a OneSignal App**

1. Go to [OneSignal Dashboard](https://dashboard.onesignal.com/) and sign in with your account.

2. Click **"New App/Website"** to start the setup.

3. Enter your app name, organization details.

4. Select **"Google Android (FCM)"** and click **"Next: Configure Your Platform"**.

**Step 2: Obtain the Service Account File from Firebase**

Now, you need to obtain the Service Account file from Firebase. Follow these steps:

1. Go to [Firebase Console](https://console.firebase.google.com/) and select the app you created.

3. Navigate to **Project Settings** > **Service Accounts**.

4. Click **"Generate new private key"** and confirm. The service account file will be downloaded.

**Step 3: Complete OneSignal Setup**

1. Upload the service account JSON file you downloaded from Firebase.

2. Click **Save & Continue**.

3. Select **Native Android** and click **Save & Continue**.

4. Click **Done** to finish the setup.

For a detailed, step-by-step guide, watch the walkthrough video.

<div class="video-container"><iframe src="https://www.youtube.com/embed/MHhVM7oa91M?si=1Dr6JP1fwsV4oucY" title="YouTube video player" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe></div>

## Enable OneSignal in NoSyntax

To enable OneSignal in NoSyntax, follow these steps:

1. In the OneSignal dashboard, go to **Settings** > **Keys & IDs**.

2. Copy the **OneSignal App ID** and **Rest API Key**.

3. In the NoSyntax panel, navigate to **Settings** > **Integrations** > **OneSignal**.

4. Toggle the **Enable** switch.

5. Paste the **OneSignal App ID** and **Rest API Key** into the corresponding fields.

## Manual Integration

If you've downloaded the foundation template, which is a basic setup without pre-configurations, you can manually set up OneSignal. The necessary dependencies and code are already included.

To configure OneSignal manually, follow these steps:

1. Open the `app-config.yml` file.

2. Update the **OneSignal App ID** under **integrations** > **onesignal** > **app_id**.

3. Rebuild the project to apply the changes.
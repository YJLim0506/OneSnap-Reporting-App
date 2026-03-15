# OneSnap-Reporting-App
Designed specifically for Malaysians, this app makes it easy to report civic issues such as potholes, vandalized public facilities, or illegal dumping. Simply snap a photo, provide a brief description, and submit your report directly to the relevant authorities.

## Prerequisites
Before running the project, you need to download and install the following core tools:
* **Node.js**: LTS version recommended.
* **Java Development Kit (JDK)**: JDK 17 is recommended for modern React Native projects.
* **Android Studio**: Even though you are using a physical device, Android Studio is required to install the necessary Android SDK, Android SDK Platform, and Build-Tools.

### Environment Variables Setup (Windows)
To allow your computer to communicate with Android devices and the emulator, you must set up your environment variables:
1. Open the Windows Windows Search bar and look for **"Edit the system environment variables"**.
2. Click on **Environment Variables...**
3. Under **User variables**, click **New...** to create a new `ANDROID_HOME` variable. Set the value to the path of your Android SDK (usually `%LOCALAPPDATA%\Android\Sdk`).
4. Select the **Path** variable, click **Edit**, and add the following paths:
   * `%LOCALAPPDATA%\Android\Sdk\platform-tools`
   * `%LOCALAPPDATA%\Android\Sdk\emulator`

## How to Run on a Physical Device
This guide assumes you are testing on an Android device. Instead of using a resource-heavy virtual machine, you can run the app directly on your phone using USB debugging.

### Step 1: Enable USB Debugging
1. On your phone, go to **Settings** > **About phone**.
2. Tap on the **Build number** 7 times to unlock Developer Options.
3. Go back to **Settings**, navigate to **Developer options** (sometimes found under System settings).
4. Scroll down and turn on **USB debugging**.

### Step 2: Connect Your Phone
1. Connect your Android phone to your computer via a USB cable.
2. A prompt should appear on your phone asking to "Allow USB debugging?". Check "Always allow from this computer" and tap **OK**.

## How to Create a New Project (For Developers)
If you are setting up this project from scratch or want to create your own React Native app without using a framework like Expo, follow these steps:

### Step 1: Initialize the Project
Use the React Native Community CLI to bootstrap a new project. Open your terminal in the directory where you want your project to live and run:
  ```bash
  npx react-native@latest init OneSnapReportingApp
  ```
### Step 2: Navigate to the Project Directory
Once the initialization process is complete and all template files are generated, move into your new project folder:
  ```bash
  cd OneSnapReportingApp
  ```
### Step 3: Verify Your Setup
Before running the app, ensure your physical Android device is connected and USB debugging is enabled. You can verify your device is recognized by running:
  ```bash
   adb devices
  ```
### Step 4: Install Dependencies
If you have just cloned this repository, navigate into the project folder and install the required packages:
```bash
npm install



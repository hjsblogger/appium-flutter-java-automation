<img width="1000" height="500" alt="Image" src="https://github.com/user-attachments/assets/9f878858-8100-4f21-aeb3-b838797fddb5" />
<div align="center">Image generated using AI</a></div>
<br/>

*This repo draws inspiration from the [Flutter Demo](https://github.com/mfaisalkhatri/flutter-lambdatest-demo/) repository created by Mohammad Faisal Khatri. Thanks for your awesome work!*

In this 'Appium Flutter Java Automation' repo, we have covered the nuances of automating Flutter application testing using the following Appium drivers:
- [Appium Flutter Driver](https://github.com/appium/appium-flutter-driver)
- [Appium Flutter Integration Driver](https://github.com/AppiumTestDistribution/appium-flutter-integration-driver/)

The testing is performed on Real Device Cloud infrastructure provided by [TestMu AI](https://www.testmu.ai/)

## Steps for test execution

**Step 1**

Fetch the TestMu AI Credentials from the [TestMu AI Profile Section](https://accounts.lambdatest.com/security/username-accesskey) section. Export the environment variables *LT_USERNAME* and *LT_ACCESS_KEY* by triggering the following commands on the terminal:

For macOS:

```bash
export LT_USERNAME=LT_USERNAME
export LT_ACCESS_KEY=LT_ACCESS_KEY
```

For Linux:

```bash
export LT_USERNAME=LT_USERNAME
export LT_ACCESS_KEY=LT_ACCESS_KEY
```

For Windows:

```bash
set LT_USERNAME=LT_USERNAME
set LT_ACCESS_KEY=LT_ACCESS_KEY
```

Alternatively, update the TestMu AI Credentials - [LT_USERNAME](https://github.com/hjsblogger/appium-flutter-java-automation/blob/main/Makefile#L19) and [LT_ACCESS_KEY](https://github.com/hjsblogger/appium-flutter-java-automation/blob/main/Makefile#L20) in Makefile.

**Step 2**

For testing, we have used the open-source [Provider Shopper Flutter sample app](https://github.com/flutter/samples/tree/main/provider_shopper). The app is built for testing with the Flutter Driver and Flutter Integration Driver respectively.

You can download the Apps from the following locations:

- [Provider Shopper Flutter sample app - Flutter Driver](https://drive.google.com/file/d/1iu71pDWVXIp-c1U4nvJpoVzhLWD1dR9F/view?usp=drive_link)
- [Provider Shopper Flutter sample app - Flutter Integration Driver](https://drive.google.com/file/d/1waRST8fzE6y4BpbSo15L8d3M2Kl-mP-2/view?usp=drive_link)

The app needs to be uploaded to the TestMu AI cloud storage. For this, navigate to the [App Live App Dashboard](https://applive.lambdatest.com/app), select the app, and click the 'Upload' button.

<img width="1503" height="827" alt="Image" src="https://github.com/user-attachments/assets/2801d02b-9add-4390-bc47-617f4233c092" />


Now that both the apps are uploaded to the TestMu AI cloud storage, retrieve the App ID by clicking on the *Settings* button next to uploaded app:

<img width="1488" height="692" alt="Image" src="https://github.com/user-attachments/assets/21a04652-104c-4764-9d50-6a4c2f77bad7" />

Next, update the App ID in the test files:

- [Flutter Driver Test Code](https://github.com/hjsblogger/appium-flutter-java-automation/blob/main/src/main/java/AndroidApp_Flutter.java#L18)
- [Flutter Integration Driver Test Code](https://github.com/hjsblogger/appium-flutter-java-automation/blob/main/src/main/java/AndroidApp_Flutter_Integration.java#L17)

**Step 3**

Run the *make clean* command on the terminal to clean the temporary files

```bash
make clean
```

Run the *make build* command on the terminal to build the automation project

```bash
make build
```

<img width="1480" height="583" alt="Image" src="https://github.com/user-attachments/assets/4a834990-70b0-4a21-a5e6-2b97354d687d" />
<br/><br/>

**Step 4 - Automation with Appium Flutter Integration Driver**

Trigger the command ```make flutter-integration-driver-test``` to test Flutter app on the TestMu AI cloud grid using the Appium Flutter Integration Driver.

<img width="1485" height="591" alt="Image" src="https://github.com/user-attachments/assets/38ba2905-7c9a-49d9-9a3d-2ac5d86b821a" />

<img width="1039" height="408" alt="Image" src="https://github.com/user-attachments/assets/590cb2b2-d524-419b-aad3-48ebbc68806f" />

Navigate to the [TestMu AI Automation Dashboard](https://automation.lambdatest.com/) to check the status of the test execution.

<img width="1495" height="827" alt="Image" src="https://github.com/user-attachments/assets/712ccc20-d8e5-493c-b086-5cebcb052207" />
<br/><br/>

**Step 5 - Automation with Appium Flutter Driver**

Trigger the command ```make flutter-driver-test``` to test Flutter app on the TestMu AI cloud grid using the Appium Flutter Driver.

<img width="1488" height="491" alt="Image" src="https://github.com/user-attachments/assets/68c95bd2-25bb-4cb5-8303-f81a61106e95" />

<img width="1132" height="454" alt="Image" src="https://github.com/user-attachments/assets/4a591891-ec0d-4a5e-a257-8afac9e8807b" />

Navigate to the [TestMu AI Automation Dashboard](https://automation.lambdatest.com/) to check the status of the test execution.

<img width="1495" height="827" alt="Image" src="https://github.com/user-attachments/assets/ff35b0d0-98a0-4730-b89f-e3e36ea90ac0" />
<br/>

## :question: Need Assistance?
Feel free to fork the repo and contribute to make it better! Email to [himanshu[dot]sheth[at]gmail[dot]com](mailto:himanshu.sheth@gmail.com) for any queries or ping me on the following social media sites:

<b>LinkedIn</b>: [@hjsblogger](https://linkedin.com/in/hjsblogger)<br/>
<b>Twitter</b>: [@hjsblogger](https://www.twitter.com/hjsblogger)

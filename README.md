# Mobile fragmentation


[Hybrid, Native, and PWAs: Testing your mobile apps for compatibility](https://www.browserstack.com/blog/hybrid-native-pwas-testing-your-mobile-apps-for-compatibility/)

Mobile fragmentation affects all apps—some more than others.
Usually, the more dependencies an app has on native device features/APIs, the harder it is to make it work seamlessly on every user’s device.
However, two apps can offer the same features and still not be affected to the same degree by fragmentation. It depends on how they’re built. 

### Prepare Apps for Mobile Fragmentation
Common tests for apps (and how QAs go about performing them) are covered in a [post about mobile app testing](https://www.browserstack.com/blog/mobile-app-testing/).
But to prepare your apps for mobile fragmentation, you’ll have to go the extra mile.

Use the app analytics with the [Test on the Right Devices](https://www.browserstack.com/test-on-the-right-mobile-devices) report, and draw up a list of mobile devices, OS versions, and browsers (for PWAs) that will cover more than 80% of your audience and target market. Then validate UI, functionality, and performance (regardless of the type of app) on:

- Different mobile screen sizes and resolutions (especially the outliers, like iPhone X).
- Flaky network conditions, particularly for apps with offline access and Lite mobile versions.
- Different Android and iOS versions, based on market share (and crash reports). This includes testing on Android OEMs’ custom skins, like OneUI (OnePlus), MiUI (Xiaomi), EMUI (Huawei) and so on.

Additionally, since different app types will be affected to varying degrees by fragmentation, remember to:

- Test __hybrid__ app functionalities on mobile OS, as well as mobile browser versions. Any features in the new versions of Chrome-for-Android and Safari-on-iOS may carry over to their WebView as well.
- Test __native__ apps on real mobile devices for battery overconsumption and hardware performance issues, since emulators and simulators will not be able to capture them.
- Test __PWA__ functionalities on mobile OS-browser combinations, and if native device features are used, test on real mobile devices before release.

The three types of mobile apps interact differently with the device. Due to the differences in browsers, OS, and hardware, the interactions can become unpredictable.

To avoid gaps in your UX, remember to account for these differences while building your test plan. The most important point to remember is the one we started with—Mobile fragmentation affects all apps, some more than others. 

-------

[Testing for Fragmentation: The perfect cross-device test strategy for mobile](https://www.browserstack.com/blog/perfect-test-strategy-for-mobile/)
[Testing for Fragmentation: Understanding Browser, OS and Device Fragmentation](https://www.browserstack.com/blog/understanding-browser-os-and-device-fragmentation/)

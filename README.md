# <img src="https://user-images.githubusercontent.com/70295997/213381298-2f724904-0bf5-47f4-a88d-d61272cb1435.png" width=40> Mobile fragmentation

<img width="400" src="https://user-images.githubusercontent.com/70295997/213381929-2f725045-80de-4118-8717-b60dbd79e3cf.png">

Mobile fragmentation refers to the diverse range of hardware and software configurations that exist among mobile devices, such as smartphones and tablets. This can include differences in screen size, processor type and speed, amount of memory, and version of the operating system. Mobile fragmentation can cause [interoperability](https://github.com/lana-20/interoperability) issues. For example, it can make it difficult for developers to create apps that work consistently across all devices, and can also pose challenges for users in terms of accessing certain features or finding compatible apps. In general, the more fragmented a mobile ecosystem is, the more difficult it is for developers to create apps and for users to have a consistent experience across devices.

The [Android operating system (OS)](https://github.com/lana-20/android-distro) is vast, with different screen sizes, resolutions, and capabilities ranging across versions and devices. The list of versions which the system supports (including updates) is much bigger than that of iOS. In addition to vanilla Android configs on various devices, testers and developers also deal with [skins](https://www.androidauthority.com/android-skins-945375/), such as Samsung's One UI, Google’s Pixel UI, OnePlus’ Oxygen OS, Motorola’s My UX and Xiaomi MIUI.

![image](https://user-images.githubusercontent.com/70295997/205458610-42c374f3-d427-470a-aae3-90e0013cb58c.png)

Source: [Guide: Browser and Device Fragmentation](https://github.com/lana-20/mobile-fragmentation/blob/main/Guide%2B-%2BBrowser%2Band%2BDevice%2BFragmentation.pdf)

There are 24,000 distinct Android configurations in the wild.

<img src="https://user-images.githubusercontent.com/70295997/211403279-bbe64c3d-9796-4b68-84df-5748db3f7dc5.png" width=800>

Source: [Report Finds 24K Distinct Android Devices](https://www.pcmag.com/news/report-finds-24k-distinct-android-devices)
_____

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
- Different Android and iOS versions, based on market share (and crash reports). This includes testing on Android OEMs’ custom skins, like OneUI (Samsung), MiUI (Xiaomi), EMUI (Huawei) and so on.

Additionally, since different app types will be affected to varying degrees by fragmentation, remember to:

- Test __hybrid__ app functionalities on mobile OS, as well as mobile browser versions. Any features in the new versions of Chrome-for-Android and Safari-on-iOS may carry over to their WebView as well.
- Test __native__ apps on real mobile devices for battery overconsumption and hardware performance issues, since emulators and simulators will not be able to capture them.
- Test __PWA__ functionalities on mobile OS-browser combinations, and if native device features are used, test on real mobile devices before release.

The three types of mobile apps interact differently with the device. Due to the differences in browsers, OS, and hardware, the interactions can become unpredictable.

To avoid gaps in your UX, remember to account for these differences while building your test plan. The most important point to remember is the one we started with—Mobile fragmentation affects all apps, some more than others. 

-------

[Testing for Fragmentation: The perfect cross-device test strategy for mobile](https://www.browserstack.com/blog/perfect-test-strategy-for-mobile/)

[Testing for Fragmentation: Understanding Browser, OS and Device Fragmentation](https://www.browserstack.com/blog/understanding-browser-os-and-device-fragmentation/)

[What is Android fragmentation, and can Google ever fix it?](https://www.digitaltrends.com/mobile/what-is-android-fragmentation-and-can-google-ever-fix-it/)

[BrowserStack Fragmentation Blog](https://www.browserstack.com/blog/tag/fragmentation-testing/)

[The many flavors of Android: A look at the major Android skins](https://www.androidauthority.com/android-skins-945375/)

[Don't be shy, Android skins. Flaunt your best features.](https://www.androidauthority.com/android-skins-commentary-3093771/)

-------


### Mobile Platform

Worldwide Statistics

Last 12 Months (Nov 2021 - Nov 2022) | [2022 Stats updated on 12/31/2022](https://github.com/lana-20/mobile-distro-global-2022)

[Vendor Market Share](https://gs.statcounter.com/vendor-market-share/mobile/worldwide/#monthly-202111-202211-bar)
![StatCounter-vendor-ww-monthly-202111-202211-bar](https://user-images.githubusercontent.com/70295997/204199695-51654fef-91ce-4d63-a7fa-68cf45634844.png)
![image](https://user-images.githubusercontent.com/70295997/204201991-c33d0ce7-0947-40f2-86c4-d3f716e4bfab.png)


[Operating System Market Share](https://gs.statcounter.com/os-market-share/mobile/worldwide#monthly-202111-202211-bar)
![StatCounter-os_combined-ww-monthly-202111-202211-bar](https://user-images.githubusercontent.com/70295997/204199891-4d724fd3-7d56-488b-82e4-cb6fc9b7aa22.png)
![image](https://user-images.githubusercontent.com/70295997/204201606-9f310df0-54a4-41e8-b596-86d2745b861d.png)


[Screen Resolution Stats](https://gs.statcounter.com/screen-resolution-stats/mobile/worldwide#monthly-202111-202211-bar)
![StatCounter-resolution-ww-monthly-202111-202211-bar](https://user-images.githubusercontent.com/70295997/204200155-0bb5c104-9911-4976-b485-4a8c2181aac6.png)
![image](https://user-images.githubusercontent.com/70295997/204201195-ee0e190a-fa31-4383-ba48-bb494dcefc6c.png)

See also the [08/01/2022 Mobile OS Market Share](https://miro.com/app/board/uXjVOicYjsk=/) diagram:

<img width="400" src="https://user-images.githubusercontent.com/70295997/213385857-67361543-4db5-48f4-8246-e617fc3a42b8.png">




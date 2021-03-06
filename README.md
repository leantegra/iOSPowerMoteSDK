# BLE Beacon SDK for iOS #

BLE Beacon SDK for iOS is a library that allows interaction with any iBeacon / Eddystone compatible devices, including both Leantegra beacons and 3rd-party devices from other vendors (e.g. Estimote, Kontakt.io).

Features:
- Based on Apple Core Location and Apple Core Bluetooth Frameworks;
- WiBeat management: connect\disconnect, read\write all info from nearby device;
- WiBeat ranging: scanning for nearby devices, filtering by specified properties, distance to device (IMMEDIATE, NEAR, FAR zones);
- WiBeat monitoring: monitors Enter\Exit events for predefined regions that can be defined by multiple rules (UUID, distance, zone, Major, Minor etc.);
- Integration with Leantegra CMS (notifications, multi-rules, analytics).

## Installation

### Manual installation

1. Add [LeantegraSDK.framework](https://github.com/leantegra/iOSWiBeatSDK/blob/master/WiBeatSDK/LeantegraSDK.framework) into Xcode project; 
2. Add Apple's CoreLocation and Apple's CoreBlueooth frameworks into Xcode project;
3. For WiBeat Monitoring feature, if You are using iOS 11 as your base SDK, add NSLocationAlwaysAndWhenInUseUsageDescription and [NSLocationWhenInUseUsageDescription](https://developer.apple.com/library/content/documentation/General/Reference/InfoPlistKeyReference/Articles/CocoaKeys.html#//apple_ref/doc/uid/TP40009251-SW26) keys in your Info.plist file.
   If You are using iOS 10 and lower as your base SDK, add [NSLocationAlwaysUsageDescription](https://developer.apple.com/library/ios/documentation/General/Reference/InfoPlistKeyReference/Articles/CocoaKeys.html#//apple_ref/doc/uid/TP40009251-SW18) or [NSLocationWhenInUseUsageDescription](https://developer.apple.com/library/content/documentation/General/Reference/InfoPlistKeyReference/Articles/CocoaKeys.html#//apple_ref/doc/uid/TP40009251-SW26) key in your Info.plist depending on your needs;
4. For WiBeat Monitoring feature, add [bluetooth-central](https://developer.apple.com/library/content/documentation/NetworkingInternetWeb/Conceptual/CoreBluetooth_concepts/CoreBluetoothBackgroundProcessingForIOSApps/PerformingTasksWhileYourAppIsInTheBackground.html#//apple_ref/doc/uid/TP40013257-CH7-SW7) property key;
5. For WiBeat Monitoring feature, enable "Uses Bluetooth LE accessories" checkbox in Xcode target settings – TARGETS/Capabilities/Background Modes.

## How to use

### Documentation

Apple Docs for WiBeat SDK you can find [here](http://leantegra.github.io/iOSWiBeatSDK/AppleDocs/).

### Demo Applications

Demo applications you can find [here](https://github.com/leantegra/iOSWiBeatSDK/tree/master/Demos).

### Changelog

The list of changes in WiBeat SDK for iOS located in [CHANGELOG](https://github.com/leantegra/iOSWiBeatSDK/blob/master/CHANGELOG.md).

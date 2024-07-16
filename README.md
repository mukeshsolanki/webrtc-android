# WebRTC Binaries for Android

![GitHub Release](https://img.shields.io/github/v/release/mukeshsolanki/WebRTC-android)
![Maven Central Version](https://img.shields.io/maven-central/v/io.github.mukeshsolanki/webrtc-android)

This repository contains the unofficial distribution of WebRTC framework binaries for Android.

Since version M80, Google has deprecated their mobile binary libraries distributions (Was officially using the JCenter). To get the most up-to-date WebRTC library, you can compile it on your own, or you can use precompiled binaries from here.

## 📦 Releases
The binary releases correspond with official Chromium releases and branches as specified in the Chromium dashboard.

## 💡 Things to know
All binaries in this repository are compiled from the official WebRTC source code without any modifications to the source code or the output binaries.

## 📢 Requirements
minSdkVersion = 21

## 📀 Binaries included
* arm64-v8a
* armeabi-v7a
* x86
* x86_64

## 🚚 Installation

### Maven
The latest release is available on [Maven Central](https://central.sonatype.com/artifact/io.github.mukeshsolanki/webrtc-android)

**Gradle Groovy DSL**

```
implementation 'io.github.mukeshsolanki:webrtc-android:<latest-version>'
```

**Gradle Kotlin DSL**

```
implementation("io.github.mukeshsolanki:webrtc-android:<latest-version>")
```

**Manual**

* Download the AAR from the releases section.
* Copy the AAR file into a libs folder inside your app folder.
* Include the following line in the dependencies section of your build.gradle.kts file

```
implementation(files("libs/libwebrtc-<latest-version>.aar"))
```

### Proguard

```
-keep class org.webrtc.** { *; }
```

## 🛠 Compile your own WebRTC AAR

If you wish to compile your own WebRTC AAR, please refer to the following official guide: https://webrtc.googlesource.com/src/+/refs/heads/main/docs/native-code/android/

## 📃 License

WebRTC License: https://webrtc.org/support/license

# Assignment 1: Android Theory & Publishing Guide

This repository contains the theory assignment and practical demonstration for publishing an Android application. The document covers APK versioning, generating a signed build, and the complete workflow for publishing to the Google Play Console.

## 📄 File Included
- **Assignment1 Android Theory.pdf** - The complete detailed report.

## 📌 Overview
Publishing an Android app involves more than writing code. This assignment explains the essential stages: assigning proper version numbers, digitally signing the app for author verification, and uploading it to the Google Play Console along with a store listing, privacy policy, and required declarations.

## 📚 Key Topics Covered

### 1. APK Versioning
- **versionCode vs versionName**: Explanation of internal version tracking versus user-facing version labels.
- **Importance**: Why every new release must have a higher `versionCode` to avoid rejection by the Google Play Console.
- **Location in Android Studio**: How to find and edit these values in the `build.gradle` (Module: app) file.

### 2. Generating a Signed Build
- **Keystore (.jks) File**: What it is and why it is critical for proving developer identity and securing future updates.
- **APK vs. AAB**: The difference between installable packages and publishing formats. Google Play now requires new apps to be published as AAB files.
- **Step-by-Step Guide**: Detailed instructions (with screenshots) on how to generate a signed release file in Android Studio, including creating a new keystore and selecting the release build variant.

### 3. Publishing to Google Play
- **Developer Account Requirements**: The one-time $25 fee, identity verification, and the mandatory closed testing requirement (12 testers for 14 continuous days) for new personal accounts.
- **Publishing Steps**: From creating the app and completing the dashboard tasks to preparing the store listing and rolling out a production release.
- **Common Errors & Rejections**: How to avoid issues like duplicate versionCodes, using `com.example`, missing privacy policies, and outdated target API levels.

## 🛠️ Practical Task Demonstration
A basic "Hello World" application (`MyApplication`) was created in Android Studio with the following specifications:
- **Application ID**: `com.areeba.hellorelease`
- **Version**: `versionCode 1` and `versionName "1.0"`
- **SDK**: `minSdk 24` and `targetSdk 37`

A signed release bundle (`app-release.aab`) was successfully generated and is ready for upload.

## 🚀 Play Console Publishing Plan & Current Status
- **Ready**: Application ID, versionCode, versionName, target SDK, and signed release AAB.
- **Next**: Create a personal developer account, pay the fee, and complete identity verification.
- **Testing**: Upload the AAB to a closed testing track and maintain 12 testers for 14 continuous days.
- **Release**: Apply for production access and roll out the release after Google's review.

## ✅ Conclusion
This assignment covered the full path from a finished app to a store-ready release. Understanding version codes, keystore security, and the Play Console requirements helps avoid common rejections and ensures a smooth publishing experience.

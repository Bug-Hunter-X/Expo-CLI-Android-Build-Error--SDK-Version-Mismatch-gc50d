# Expo CLI Android SDK Version Mismatch

This repository demonstrates a common error encountered when building Android projects with Expo CLI: a mismatch between the project's declared Android SDK version and the version actually installed.

## Problem:

The Expo CLI build process fails because it cannot locate or use the specified Android SDK version. This often results in errors related to missing or incompatible SDK components.

## Solution:

The solution involves verifying and correcting the Android SDK version specified in your project's `build.gradle` files to match the installed version or installing the necessary SDK version.

## How to reproduce:

1. Clone this repository.
2. Attempt to build the Android project using Expo CLI (e.g., `expo build:android`).
3. Observe the error message indicating an SDK version mismatch.

## How to fix:

1. Check the Android SDK versions installed on your system using the Android SDK Manager.
2. Ensure that the `compileSdkVersion` and `targetSdkVersion` values in the project's `build.gradle` files (both module-level and project-level) match an installed version.
3. If necessary, use the Android SDK Manager to install or update the correct SDK version.
4. Clean and rebuild the project using Expo CLI.
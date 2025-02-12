# Expo Android Build Failure: AGP Version Mismatch

This repository demonstrates a common but difficult-to-diagnose issue when building Android apps using Expo CLI. The problem stems from an incompatibility between the Android Gradle Plugin (AGP) version specified in your project's `android/build.gradle` file and the version expected or supported by the Expo build process.

## Problem
The error messages generated by Expo during the build process are often vague and don't directly point to the AGP version mismatch.  This makes troubleshooting challenging. You might see errors related to missing classes, unresolved dependencies, or general Gradle failures. 

## Solution
The solution involves carefully examining and potentially adjusting the AGP version in your project's configuration files to align with Expo's requirements.  This usually involves updating the AGP version in `android/build.gradle` and potentially `android/gradle/wrapper/gradle-wrapper.properties` to match a version known to be compatible.  In some cases, cleaning and rebuilding the project is also necessary. Refer to the `bugSolution.js` file for a demonstration.
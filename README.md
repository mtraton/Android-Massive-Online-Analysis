# Android-Massive-Online-Analysis

This repository is our attempt to make MOA (Massive Online Analysis) usable as part of Android application. We can't guarantee that it'll work in all cases.
We've simply deleted every reference to Swing functions used in MOA GUI that were involved in learning process.

Usage:

1) Build with Maven (Lifecycle->Package)
2) Import generated .jar files () to your Android application.
3) If you are using Gradle, add those lineto corresponding parts of your gradle.build file

dexOptions {
        javaMaxHeapSize "4g"
    }
    
 defaultConfig {
        multiDexEnabled = true
    }


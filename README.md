# Android-Massive-Online-Analysis

This repository is our attempt to make MOA (Massive Online Analysis) usable as part of Android application. We can't guarantee that it'll work in all cases.
We've simply deleted every reference to Swing functions used in MOA GUI that were involved in learning process.

Usage:

1) Build with Maven (Lifecycle->Package)
2) Import generated .jar files (moa-2014.05-SNAPSHOT, moa-2014.04-sources, moa-2014.04-javadoc) from target directory  to your Android application.
3) Import rest of .jar imported from Maven (java-cup-11b-runtime-2015.03.26, pentaho-package-manager-1.0.11, sizeofag-1.0.0, weka-dev-3.7.13) to your project (default position -> your .m2/repository directory or download them from this repository) (). 
3) If you are using Gradle, add those line to corresponding parts of your gradle.build file

dexOptions {
        javaMaxHeapSize "4g"
    }
    
 defaultConfig {
        multiDexEnabled = true
    }


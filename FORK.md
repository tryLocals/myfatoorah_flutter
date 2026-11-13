# About this fork

Fork of `myfatoorah_flutter` **3.3.3** from pub.dev, identical except for one change:

- `android/build.gradle`: removed `apply plugin: "kotlin-android"` and moved
  `kotlinOptions { jvmTarget = '11' }` into a top-level `kotlin { compilerOptions }`
  block, so the plugin builds under **Android Gradle Plugin 9** (which provides
  built-in Kotlin and rejects the standalone Kotlin Gradle Plugin).

The upstream pub.dev package still applies the deprecated Kotlin Gradle Plugin.
This fork can be retired if MyFatoorah ships an AGP 9–compatible release.

# arrow-android-failing

This repository showcases some issues when trying to use Arrow on Android projects. Basically, the builds fail complaining about missing classes on Arrow's artifacts.

[master](https://github.com/jrgonzalezg/arrow-android-failing/tree/master) branch is set up to use Java 8 as many mixed Java / Kotlin Android projects do. For this branch the build fails on the desugar task when doing `./gradlew assembleDebug`.

[java7](https://github.com/jrgonzalezg/arrow-android-failing/tree/java8) branch is set up to use Java 7 so no desugar task is run. But it still fails on the ProGuard task instead when doing `./gradlew assembleRelease`.

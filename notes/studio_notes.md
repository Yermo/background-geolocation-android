# Errors I encountered

After initially forking the project at commit:

```
yml@titan:~/Projects/background-geolocation-android$ git log
commit 3679c4273a9a7d0436fcd877a55d74e3c86e840a (HEAD -> run_tests, origin/master, origin/HEAD, master)
Author: Marian Hello <m.hello@gmail.com>
Date:   Thu Mar 28 10:56:30 2019 +0100

    updates for pkg migration
```

I ran into the following errors when trying to open the project in Android Studio 3.4

## mipsel-linux-android

```
ERROR: No toolchains found in the NDK toolchains folder for ABI with prefix: mipsel-linux-android
```

This required upgrading gradle.

See:

https://stackoverflow.com/questions/35128229/error-no-toolchains-found-in-the-ndk-toolchains-folder-for-abi-with-prefix-llv

## minSdk

```
The minSdk version should not be declared in the android manifest file. You can move the version from the manifest to the defaultConfig in the build.gradle file.
```

I clicked: "Remove minSdkVersion and sync project"

The "Refactoring Preview" opened.

I clicked 'Do Refactor'

## Android SDK Build Tools

```
The specified Android SDK Build Tools version (27.0.3) is ignored
```

I clicked: 'Remove Build Tools version and sync project'

and then 'Do Refactor'

## Tests

I wanted to get the initial tests running. I may have made some mistake, but at first there were no options to run any
tests. I eventually stumbled upon running the tests from the command line using:

```
./gradlew test
```

After that, I noticed from the Android drop down in the upper left, that the Run Tests options were now available and work.


### 报错

```
react-native run-android
```

运行报错：

```
info JS server already running.
info Building and installing the app on the device (cd android && ./gradlew app:installDebug)...
error Could not install the app on the device, read the error above for details.
Make sure you have an Android emulator running or a device connected and have
set up your Android development environment:
https://facebook.github.io/react-native/docs/getting-started.html
error spawnSync ./gradlew EACCES
```
解决办法
```
chmod 755 android/gradlew
```

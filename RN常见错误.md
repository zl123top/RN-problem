### 报错

运行报错：

```
zhanglinMac:BOSPadProject zhanglin$ 
zhanglinMac:BOSPadProject zhanglin$ cd android && ./gradlew clean
bash: ./gradlew: Permission denied
zhanglinMac:android zhanglin$ react-native run-androidCommand `run-android` unrecognized. Make sure that you have run `npm install` and that you are inside a react-native project.
zhanglinMac:android zhanglin$ cd ../
zhanglinMac:BOSPadProject zhanglin$ react-native run-android
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

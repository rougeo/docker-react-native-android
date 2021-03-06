# docker-react-native-android
A 🐳 docker image for building ⚛ React Native Apps (Android only)

[![Travis](https://img.shields.io/travis/jaydp17/docker-react-native-android.svg)](https://travis-ci.org/jaydp17/docker-react-native-android)
[![](https://images.microbadger.com/badges/image/jaydp17/react-native-android.svg)](https://microbadger.com/images/jaydp17/react-native-android)


### Installed Packages
- Open JDK 8
- Gradle v3.3
- Android SDK 23, 25 & 26
- Android Build Tools 23.0.1, 25.0.2, 26.0.1
- Android Tools (tools, platform-tools, extras)
- Google Extras

## How to use?
```sh
# The below will run the container and open up a bash session in side the container
$ docker run --rm -it -v /path/to/my/react-native-app:/app jaydp17/react-native-android:latest bash

# cd into the project
$ cd /app

# install npm modules
$ yarn

# Now cd into the android folder
$ cd android

# build the app
$ ./gradlew assembleRelease
```
Once the build is successful, you can find the apk in `app/build/outputs/apk/` directory.

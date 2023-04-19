# Install Native Module
1. Get Ubuntu WSL running
2. Install node
3. Install yarn
4. Install expo with Yarn
5. Run npx create-expo-module my-module-name
6. You can only build Android, to do so install the Android SDK, see below

## Install Android SDK
1. sudo add-apt-repository ppa:webupd8team/java
2. sudo apt update
3. sudo apt install openjdk-8-jdk
4. wget https://dl.google.com/android/repository/commandlinetools-linux-6200805_latest.zip
5. mkdir -p Android/Sdk
6. unzip commandlinetools-linux-6200805_latest.zip -d Android/Sdk
7. export ANDROID_HOME=$HOME/Android/Sdk
8. export PATH="$ANDROID_HOME/emulator:$ANDROID_HOME/tools:$ANDROID_HOME/tools/bin:$ANDROID_HOME/platform-tools:$PATH"
9. sudo apt install sdkmanager
10. sudo sdkmanager --sdk_root=${ANDROID_HOME} "tools"
11. sudo sdkmanager --update
12. sudo sdkmanager --list
13. sudo sdkmanager "build-tools;28.0.3" "platform-tools" "platforms;android-28" "tools"
14. sudo sdkmanager --licenses
15. sudo apt install gradle

## Build Module

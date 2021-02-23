# FLUTTER

## Download

https://flutter.dev/docs/get-started/install/macos

download the archive in your ~/Downloads folder.

## Install Flutter
On a Mac tilde character "~" is `Option+n` and it is a shortcut
for the $HOME directory.

- create a tools directory:
    `mkdir ~/tools`
-  unzip the archive and extract the content to ~tools
    `unzip -o -q flutter_macos_1.22.6-stable.zip -d ~/tools/`
- check if flutter folder has been extracted in ~/tools
    `ls -lah ~/tools`
- change directory to $HOME (which is ~)
    `cd`
- append to the PATH so that MacOS can find the flutter binary
    `echo 'export PATH="$PATH:$PWD/tools/flutter/bin"' >> .zshrc`
    note:
    - zsh is supposed to be the default shell on MacOS in 2021
    - `>> .zshrc`  means append at the end of the file .zshrc which contains configuration for zsh
    - $PATH contains previous content of variable PATH
    - $PWD means path to working directory (current directory you are in)
- make sure you apply new config
    `source .zshrc`
- check if binary has been added, should give you the path to flutter binary
    `which flutter`
- check your flutter installation
    `flutter doctor`


## Platform setup

https://flutter.dev/docs/get-started/install/macos#platform-setup

## Install XCode on Mac

https://developer.apple.com/download/

## Install Android Studio

- download android studio
https://developer.android.com/studio/index.html

- flutter android setup
https://flutter.dev/docs/get-started/install/macos#android-setup

- accept android licenses:
`flutter doctor --android-licenses`

- install flutter/dart plugins for android studio
Android Studio > preferences > Plugins: Select Flutter in the list
install then restart Android Studio.

- Virtual Device
Android Studio > Tools > Android > AVD Manager and select Create Virtual Device…

- flutter looks for the plugins in the wrong folder since the update, need a symlink to let it find the plugins
`ln -s ~/Library/Application\ Support/Google/AndroidStudio4.1/plugins ~/Library/Application\ Support/AndroidStudio4.1`

## Setup VSCode for Flutter

Flutter Plugin:
https://marketplace.visualstudio.com/items?itemName=Dart-Code.flutter




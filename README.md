# APE User Guider


## Build

1. Install Android SDK, add `build-tools` and `platform-tools` to `$PATH`, and make sure the command `dx` is invocable in your shell.
    * Mac OS: `ANDROID_HOME` can be found at `/Users/<your-name>/Library/Android/sdk/`
    * You can save the following two lines into a file named AndroidSDK and put the file into `/etc/path.d`. Next time when you open a new terminal.

        /Users/tianxiaogu/Library/Android/sdk/build-tools/25.0.3
        /Users/tianxiaogu/Library/Android/sdk/platform-tools

2. Install `ant` <http://ant.apache.org/>
    * Mac OS: `brew install ant`
3. Install a JDK 1.7 or higher
4. Run command `ant` to build the project. You will find a file named `ape.jar`.


## Install

1. Upload the `ape.jar` to `/sdcard/`
    * `adb push ape.jar /sdcard/`
2. Update the `ape` script for invoking the ape in the phone.
    * `adb push ape /sdcard/`


## Run

1. Via `adb shell`
    * `adb shell ape`
    * `ape` inherits all options from Monkey.

2. Via the `ape.py` from your local shell.
    * `./ape.py`


# Micro-for-Android
*-Micro Text Editor for Android-*

#### **Micro-for-Android** is a port of the [`Micro Text Editor`](https://github.com/zyedidia/micro) for Android.
This application is available in three variants:
> 1. Containing only the text editor.
> 2. Containing the text editor and the `GNU Compiler Collection (GCC v10.2.0)`.
> 3. Containing the text editor, `GCC v10.2.0` and `Python v3.6.6`.

## How does it work ?

• This application contains a `Shell Script` embedded into a stripped-down version of [`Terminal Emulator for Android`](https://github.com/jackpal/Android-Terminal-Emulator) which is executed at runtime.
• The shell script copies all required files from the internal storage and sets up the environment.

## Installation

Instructions to install the third variant of the application, i.e. the one containing GCC and Python along Micro are given below. The installation procedure for the rest of the variants are also similar.

> 1. Unzip the archive provided in the Releases section and copy the folder inside (named `Micro`) to the `/sdcard/` location.
> 2. Install the `.apk` file inside the `Micro` folder.
> 3. Launch the application, provide the permissions required and let it set up the environment. After the setup, the Micro Text Editor Window shows up.
>

#### ***Note:***
***• Do not rename the folder named Micro before installing the application. You can delete the `/sdcard/Micro` folder after launching the app for the first time.***
***• For best experience, in the `Preferences` menu of the application, increase the `Font size` to at least `14`, check the options to `Send mouse events` and to `Close window on exit`. You can also change the `Terminal type` to `screen-256color` for better color support.***

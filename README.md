# Micro-for-Android
*-Micro Text Editor for Android-*


#### **Micro-for-Android** is a port of the [`micro-editor`](https://github.com/zyedidia/micro) for Android.
This application is available in three variants:
> 1. Containing only the text editor.  
> 2. Containing the text editor and the `GNU Compiler Collection (GCC v10.2.0)`.  
> 3. Containing the text editor, `GCC v10.2.0` and `Python v3.6.6`.  

## How does it work ?

• This application contains a `Shell Script` embedded into a stripped-down version of [`Terminal Emulator for Android`](https://github.com/jackpal/Android-Terminal-Emulator) which is executed at runtime.  
• The shell script copies all required files from the internal storage and sets up the environment during first launch.  

## Installation

Instructions to install all variants of the application are similar and are given below.

> 1. Unzip the archive provided in the Releases section and copy the folder inside (named `Micro`) to the `/sdcard/` location.  
> 2. Install the `.apk` file inside the `Micro` folder.  
> 3. Launch the application, provide the permissions required and let it set up the environment. After the setup, the Micro Text Editor Window shows up.  
>

#### ***Note:***  
***• Do not rename the folder named Micro before installing the application. You can delete the `/sdcard/Micro` folder after launching the app for the first time.***  
***• For best experience, in the `Preferences` menu of the application, increase the `Font size` to at least `14`, check the options to `Send mouse events` and to `Close window on exit`. You can also change the `Terminal type` to `screen-256color` for better color support.***  

## Usage

All general keybindings and commands for the micro-editor apply in this application too. Some useful keybindings are given below:  
> • Ctrl + q - Exit the editor window  
> • Ctrl + e - Run micro-editor's commands  
> • Ctrl + b - Run commands in the Android shell  

**Note:**  
• The best method to access the Android shell through this application is using the `Ctrl + b` keybinding and typing `sh`.  
• All GCC & Python tools can be invoked from the shell.  
• All GCC tools are present in the `$HOME/portable` folder in the form of executable shell scripts (Note that the `gcc` command is not valid in this application; use `cc` instead.)  
• Read the shell scripts `cc` and `g++` to know more about the argumemts passed to gcc and g++ by default (-Os -s -fPIE -pie).  
• Core utilities are provided from the `/system/bin` folder and the `busybox` utility provided inside $HOME.  
• All Python tools are present inside the `$HOME/py/files/bin` folder.  
• To invoke the Python Shell, type `python` in the shell prompt. To install external libraries, invoke the `pip` console with the command `pipconsole` and type pip commands there (for eg. pip3 install argparse)  
• To execute a Python script, type `python /path/to/script(.py)` into the shell prompt.  


## Notice

*-This application contains portions of the [`micro-editor`](https://github.com/zyedidia/micro) project, [`qpython3`]( https://github.com/qpython-android/qpython3) project and the application [`GCC plugin for C4droid`](https://play.google.com/store/apps/details?id=com.n0n3m4.gcc4droid&hl=en_US&gl=US) and copyrights for all those components remain with their respective authors-*  

Note: This application provides very basic functionality w.r.t GCC and Python. Compatibility of libraries and advanced functionalities of all the components are largely untested.

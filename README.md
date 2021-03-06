KA Lite Installer for Windows
==========

This project provides a smoother way to install and run KA Lite in a Windows Machine.
Also see: [compiled bundle and video overview](http://kalitewiki.learningequality.org/installation/windows-installation).

---
#### This project was built using the following software:
* Inno Setup 5.5.3
* Inno Script Studio 1.0.0.24
* Microsoft Visual Studio Express 2012
* Git (note: install with the option to place the `git` executable in the path, so it can be run within `cmd`)

---
#### Instructions to build "KALiteSetup.exe":
* Clone this repository;
* Open `cmd` -- the Windows command prompt;
* Run `git submodule update --init`
* Run `make.vbs` and wait until the file is built;
* The output file named "KALiteSetup.exe" will appear within this project folder.

---
##### To clone this repository, run the following line:
    git clone --recursive https://github.com/learningequality/ka-lite-windows.git
###### (the `--recursive` is required due to the `ka-lite` submodule)

---
##### If you wish to build it using Wine, run the following line:
    wine inno-compiler/ISCC.exe installer-source/KaliteSetupScript.iss

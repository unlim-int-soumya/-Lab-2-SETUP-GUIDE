# -Lab-2-SETUP-GUIDE
Setup Gide for SDK on your Windows Machine for Raspberry Pi Pico
This lab's prelab section covered how to become familiar with the various terminals and text editors available.

However, in this lab, we had to install the SDK (Software Development Kits) for C/C++ in order to configure our PC for RP2040 development using Pico.

Since we used a Windows PC, we had to follow the steps below to install the C/C++ SDK, browse the pico-examples repository, and successfully run our first "hello_usb.c"  program.

To install C/C++ SDK on Windows 11, we needed to install the following additional tools:

1. [Arm GNU Toolchain](https://developer.arm.com/downloads/-/arm-gnu-toolchain-downloads)
2.  [CMake](https://cmake.org/download/)
3.  [Build Tools for Visual Studio 2022](https://visualstudio.microsoft.com/downloads/#build-tools-for-visual-studio-2022)
4.  [Python 3.10](https://www.python.org/downloads/windows/)
5.  [Git](https://git-scm.com/download/win)



1.ARM GNU Toolchain

- We downloaded the file 'arm-gnu-toolchain-12.2.MPACBTI-Bet1-mingw-w64-i686-arm-none-eabi.exe' mentioned below. 
![alt text](https://github.com/satyajeetburla/-Lab-2-SETUP-GUIDE/blob/main/Screen%20sort%20for%20Setup/ARM%20GNU/ARM%20GNU.png)
- We move to the next stage while the download is being completed by clicking the next button and accepting the licensing agreement. 
![alt text](https://github.com/satyajeetburla/-Lab-2-SETUP-GUIDE/blob/main/Screen%20sort%20for%20Setup/ARM%20GNU/ARM%20GNU_1.png)
![alt text](https://github.com/satyajeetburla/-Lab-2-SETUP-GUIDE/blob/main/Screen%20sort%20for%20Setup/ARM%20GNU/ARM%20GNU_2.png)
- The next step is to set the path and select a few more permissions in the checklists to configure the environment for ARM GNU. 
![alt text](https://github.com/satyajeetburla/-Lab-2-SETUP-GUIDE/blob/main/Screen%20sort%20for%20Setup/ARM%20GNU/ARM%20GNU_3.png)
-  Now installation of ARM GNU Toolchain is done.

2. CMake

- We downloaded the file '[cmake-3.24.2-windows-x86_64.msi](https://github.com/Kitware/CMake/releases/download/v3.24.2/cmake-3.24.2-windows-x86_64.msi)' mentioned below. 
![alt text](https://github.com/satyajeetburla/-Lab-2-SETUP-GUIDE/blob/main/Screen%20sort%20for%20Setup/CMake/CMake_1.png)
- Next, after accepting the licensing agreement we moved forward to path setting as shown below. 
![alt text](https://github.com/satyajeetburla/-Lab-2-SETUP-GUIDE/blob/main/Screen%20sort%20for%20Setup/CMake/CMake_2.png)
- After that the installation process occurred smoothly. 
![alt text](https://github.com/satyajeetburla/-Lab-2-SETUP-GUIDE/blob/main/Screen%20sort%20for%20Setup/CMake/CMake_3.png)

4. Build Tools for Visual Studio 2022

- In the next step of our process, We downloaded the file "[Build Tools for Visual Studio 2022](https://aka.ms/vs/17/release/vs_BuildTools.exe)" mentioned below.
![alt text](https://github.com/satyajeetburla/-Lab-2-SETUP-GUIDE/blob/main/Screen%20sort%20for%20Setup/VS%202022/VS_2022_1.png)
- Following the download, we choose the modules to be installed, as seen below. We selected to install Windows 11 SDK because we use Windows 11 Operating systems.
![alt text](https://github.com/satyajeetburla/-Lab-2-SETUP-GUIDE/blob/main/Screen%20sort%20for%20Setup/VS%202022/VS_2022_2.png)
- After this the installation procedure was completed.

6. Python 3.10

- In the next step, We downloaded the file [Latest Python 3 Release - Python 3.10.7](https://www.python.org/downloads/release/python-3107/) 
![alt text](https://github.com/satyajeetburla/-Lab-2-SETUP-GUIDE/blob/main/Screen%20sort%20for%20Setup/Python/Python%201.png)
- Following after downloading this file while installing it we chose "Add to Path" option. Because Adding Python to PATH makes it possible for you to run (use) Python from your command prompt (also known as command-line or cmd). 
![alt text](https://github.com/satyajeetburla/-Lab-2-SETUP-GUIDE/blob/main/Screen%20sort%20for%20Setup/Python/Python%202.png)

8. Git
- To follow the last step in Toolchain installation, We downloaded Git named as [64-bit Git for Windows Setup](https://github.com/git-for-windows/git/releases/download/v2.38.0.windows.1/Git-2.38.0-64-bit.exe). for our 64-bit PC.
![alt text](https://github.com/satyajeetburla/-Lab-2-SETUP-GUIDE/blob/main/Screen%20sort%20for%20Setup/Git/Git_1.png)
- Following the download, we chose a few checklists depending on our preferences.
![alt text](https://github.com/satyajeetburla/-Lab-2-SETUP-GUIDE/blob/main/Screen%20sort%20for%20Setup/Git/Git_2.png)
- And in the next step we chose Notepad as Git's default editor.
![alt text](https://github.com/satyajeetburla/-Lab-2-SETUP-GUIDE/blob/main/Screen%20sort%20for%20Setup/Git/Git_3.png)
- Following the preceding step, we enabled Git to be used from the command line as well as third-party software. 
![alt text](https://github.com/satyajeetburla/-Lab-2-SETUP-GUIDE/blob/main/Screen%20sort%20for%20Setup/Git/Git_4.png)
- Next, We selected the checkbox "Checkout as is, commit as-is" stating how Git would treat line endings in the text files. 
![alt text](https://github.com/satyajeetburla/-Lab-2-SETUP-GUIDE/blob/main/Screen%20sort%20for%20Setup/Git/Git_5.png)
- Here, We selected the terminal emulator we want to use with Git Bash. 
![alt text](https://github.com/satyajeetburla/-Lab-2-SETUP-GUIDE/blob/main/Screen%20sort%20for%20Setup/Git/Git_6.png)
- Lastly, we enabled experimental support for pseudo consoles. 
![alt text](https://github.com/satyajeetburla/-Lab-2-SETUP-GUIDE/blob/main/Screen%20sort%20for%20Setup/Git/Git_7.png)
The Toolchain installation was finally done.

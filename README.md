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
<br />


**1.ARM GNU Toolchain**<br />

- We downloaded the file 'arm-gnu-toolchain-12.2.MPACBTI-Bet1-mingw-w64-i686-arm-none-eabi.exe' mentioned below. 
![alt text](https://github.com/satyajeetburla/-Lab-2-SETUP-GUIDE/blob/main/Screen%20sort%20for%20Setup/ARM%20GNU/ARM%20GNU.png)
- We move to the next stage while the download is being completed by clicking the next button and accepting the licensing agreement. 
![alt text](https://github.com/satyajeetburla/-Lab-2-SETUP-GUIDE/blob/main/Screen%20sort%20for%20Setup/ARM%20GNU/ARM%20GNU_1.png)
![alt text](https://github.com/satyajeetburla/-Lab-2-SETUP-GUIDE/blob/main/Screen%20sort%20for%20Setup/ARM%20GNU/ARM%20GNU_2.png)
- The next step is to set the path and select a few more permissions in the checklists to configure the environment for ARM GNU. 
![alt text](https://github.com/satyajeetburla/-Lab-2-SETUP-GUIDE/blob/main/Screen%20sort%20for%20Setup/ARM%20GNU/ARM%20GNU_3.png)
-  Now installation of ARM GNU Toolchain is done.<br />

**2. CMake**<br />

- We downloaded the file '[cmake-3.24.2-windows-x86_64.msi](https://github.com/Kitware/CMake/releases/download/v3.24.2/cmake-3.24.2-windows-x86_64.msi)' mentioned below. 
![alt text](https://github.com/satyajeetburla/-Lab-2-SETUP-GUIDE/blob/main/Screen%20sort%20for%20Setup/CMake/CMake_1.png)
- Next, after accepting the licensing agreement we moved forward to path setting as shown below. 
![alt text](https://github.com/satyajeetburla/-Lab-2-SETUP-GUIDE/blob/main/Screen%20sort%20for%20Setup/CMake/CMake_2.png)
- After that the installation process occurred smoothly. 
![alt text](https://github.com/satyajeetburla/-Lab-2-SETUP-GUIDE/blob/main/Screen%20sort%20for%20Setup/CMake/CMake_3.png)<br />

**3. Build Tools for Visual Studio 2022**<br />

- In the next step of our process, We downloaded the file "[Build Tools for Visual Studio 2022](https://aka.ms/vs/17/release/vs_BuildTools.exe)" mentioned below.
![alt text](https://github.com/satyajeetburla/-Lab-2-SETUP-GUIDE/blob/main/Screen%20sort%20for%20Setup/VS%202022/VS_2022_1.png)
- Following the download, we choose the modules to be installed, as seen below. We selected to install Windows 11 SDK because we use Windows 11 Operating systems.
![alt text](https://github.com/satyajeetburla/-Lab-2-SETUP-GUIDE/blob/main/Screen%20sort%20for%20Setup/VS%202022/VS_2022_2.png)
- After this the installation procedure was completed.<br />

**4. Python 3.10**<br />

- In the next step, We downloaded the file [Latest Python 3 Release - Python 3.10.7](https://www.python.org/downloads/release/python-3107/) 
![alt text](https://github.com/satyajeetburla/-Lab-2-SETUP-GUIDE/blob/main/Screen%20sort%20for%20Setup/Python/Python%201.png)
- Following after downloading this file while installing it we chose "Add to Path" option. Because Adding Python to PATH makes it possible for you to run (use) Python from your command prompt (also known as command-line or cmd). 
![alt text](https://github.com/satyajeetburla/-Lab-2-SETUP-GUIDE/blob/main/Screen%20sort%20for%20Setup/Python/Python%202.png)<br />

**5. Git**<br />
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
<br />
**6. Getting the SDK and examples**<br />
-After that we executed the below commands in the command line. We used Powershell
![alt text](https://github.com/satyajeetburla/-Lab-2-SETUP-GUIDE/blob/main/Screen%20sort%20for%20Setup/Command%20Lines/1.png)<br />

**7. Building "Hello World" from the Command Line**<br />
-Then, from the Windows menu, we launched the Developer Command Prompt window by selecting Windows > Visual Studio 2022 > Developer Command Prompt for VS 2023 and and set the path as below. 
![alt text](https://github.com/satyajeetburla/-Lab-2-SETUP-GUIDE/blob/main/Screen%20sort%20for%20Setup/Command%20Lines/2.png)

-Before proceeding, we closed our current Command Prompt window and opened a second Developer Command Prompt session where this environment variable will now be appropriately configured.

-To construct the target, we proceeded to the pico-examples folder and generated the 'Hello World' example, as seen below. 
![alt text](https://github.com/satyajeetburla/-Lab-2-SETUP-GUIDE/blob/main/Screen%20sort%20for%20Setup/Command%20Lines/3.png)

-This generated elf, bin, and uf2 targets, which we can see within the build directory in the hello world/serial and hello world/usb directories. The UF2 binaries may be dragged and dropped straight onto an RP2040 board connected via USB to your PC.<br />
**8.SERIAL CONSOLE – SCREEN, PUTTY, ETC.** <br />
- We will install putty as our serial console.<br />
- The first thing to do is download the latest version of PuTTY. You'll want to download the Windows installer file. It is most likely that you'll need the 64-bit version. Download the file and install the program on your machine. If you run into issues, you can try downloading the 32-bit version instead. However, the 64-bit version will work on most PCs.<br />
- You'll use Windows Device Manager to determine which port the board is using. The easiest way to determine which port the board is using is to first check without the board plugged in. Open Device Manager. Click on Ports (COM & LPT). You should find something already in that list with (COM#) after it where # is a number.<br />
![alt text](https://github.com/satyajeetburla/-Lab-2-SETUP-GUIDE/blob/main/Screen%20sort%20for%20Setup/Putty%20Pict/1.png)
- Now plug in your board. The Device Manager list will refresh and a new item will appear under Ports (COM & LPT). You'll find a different (COM#) after this item in the list.<br />
![alt text](https://github.com/satyajeetburla/-Lab-2-SETUP-GUIDE/blob/main/Screen%20sort%20for%20Setup/Putty%20Pict/2.png)
- Sometimes the item will refer to the name of the board. Other times it may be called something like USB Serial Device, as seen in the image above. Either way, there is a new (COM#) following the name. This is the port your board is using.<br />
- Now you need to open PuTTY.<br />
-Under Connection type: choose the button next to Serial.<br />
-In the box under Serial line, enter the serial port you found that your board is using.<br />
-In the box under Speed, enter 115200. This called the baud rate, which is the speed in bits per second that data is sent over the serial connection. <br />
![alt text](https://github.com/satyajeetburla/-Lab-2-SETUP-GUIDE/blob/main/Screen%20sort%20for%20Setup/Putty%20Pict/3.png)
![alt text](https://github.com/satyajeetburla/-Lab-2-SETUP-GUIDE/blob/main/Screen%20sort%20for%20Setup/Putty%20Pict/4.png)

**9. Flashing and Running "Hello World"**<br />
-Connect the Raspberry Pi Pico to your Raspberry Pi using a micro-USB cable, making sure that you hold down the
BOOTSEL button to force it into USB Mass Storage Mode. 
![alt text](https://github.com/satyajeetburla/-Lab-2-SETUP-GUIDE/blob/main/Screen%20sort%20for%20Setup/Flash/IMG-0601.jpg)
- The board should automatically appear as a external drive. 
- You can now drag-and-drop the UF2 binary onto the external drive.
- The Raspberry Pi Pico will reboot, and unmount itself as an external drive, and start running the flashed code.
- You can now see hello world being printed in the serial console.
![alt text](https://github.com/satyajeetburla/-Lab-2-SETUP-GUIDE/blob/main/Screen%20sort%20for%20Setup/Flash/IMG-0602.jpg)

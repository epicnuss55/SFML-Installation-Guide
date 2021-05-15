# SFML-2.5.1 64-bit Installation Guide
SFML is a C++ GUI library used to create multimedia quick developed by [the SFML team](https://github.com/SFML). This installation guide is mainly for Visual Studios Code but should also work for other text editors or IDE's. In order to set this up and begin your project, see instructions below.
+ ***NOTE:*** The mingw64 version that comes with the installation has SFML imports, please use the given mingw64 version instead of your current version for SFML-only projects, otherwise import other libraries are required.
+ ***SFML-2.5.1 is currently the latest stable release of SFML***
## Installation Instructions
### Step 1:
clone this github repo into a folder
```git
git clone https://github.com/epicnuss55/SFML-Installation-Guide.git
```
### Step 2:
Enter `SFML Template` folder and navigate to the `mingw64` folder, move it into your C drive (or a different place you know that you're not going to move it), then enter the `mingw64` folder and navigate to `mingw64 >> bin` and copy the path. Proceed to press the windows key search up and open your `system environment`.
### Step 3:
On the newly opened `System Properties` window, press `Environment Variables`, then, in the new window, under `System variables`, find the `Path` variable and press `Edit`. Finally press the `New` button in the new Window and paste the path to the `mingw64/bin` folder you had. `OK` your way out of the `system environment`.
!()[img\SystemEnv.png]
!()[img\SystemProperties.png]
!()[img\EnvVars.png]
!()[img\EditEnvVars.png]
### Step 4:
Open `SFML_Template` (*optional*: and rename the folder) and open the folder as a project in Visual Studio Code or any other preferred text editor, open the `main.cpp` file, compile and run the template code to make sure everything is working correctly (see compiling instructions below).
## Compiling Instructions
To compile your project, open up a command prompt line on the terminal of your text editor (or use command prompt). Then open type in the following command `gcc -c main.cpp` or `gcc -c *.cpp` if you have multiple C++ files. Finally `gcc main.o -o main -lsfml-graphics -lsfml-window -lsfml-system` or `gcc *.o -o main -lsfml-graphics -lsfml-window -lsfml-system` if you have multiple object files.
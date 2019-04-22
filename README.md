# Creating and setting up CMake

## Summary

**[1. Structure](#1-structure)**
**[2. Installing CMake](#2-installing-cmake)**

## 1. Structure

We'll use the following structure for our folders and files:

.
+-- CMakeLists.txt
+-- src
| +-- _Our source files here_
+-- includes
| +-- _Our headers files here_
+-- build
| +-- _Our build files here_

That structure is very simple and makes our work more easier, we'll use it's a lot.

## 2. Installing CMake

Ok, the next step is install CMake in our machines.

#### - MacOS:

> If you're using **macOS**, follow these steps:

    - Installing with *Homebrew* **(recommended)**:
        In case you have *Homebrew* running on your computer, just type on **terminal**:

        `brew install cmake`

        ~ And the magic happens.

    - Installing manually the binary file:

        - Download the binary file in [CMake's webpage](http://cmake.org);
        - Double click the downloaded `.dmg` file to install it. In the window that pops up, drag the **CMake** icon into the *Application folder*.
        - Add this line to your `.bashrc` file: `PATH="/Applications/CMake.app/Contents/bin":"$PATH"`
        - Reload your `.bashrc` file: `source ~/.bashrc`
        - Verify the latest cmake version is installed: cmake --version
        - You can launch the CMake GUI by clicking on LaunchPad and typing cmake. Click on the CMake icon that appears.

#### - Linux:

> If you're using any **Linux** distribution, follow these steps:

    - Installing by a PPA (Upgrade to 3.2):
        - Type these commands on terminal:
            `sudo apt-get install software-properties-common`
            **`sudo add-apt-repository ppa:george-edison55/cmake-3.x`**
            `sudo apt-get update`

        > Note: You must change the bold line with the current CMake version (check out in the site)

#### - Windows:

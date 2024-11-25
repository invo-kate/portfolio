# How to install Visual Studio Code on a Chromebook

## Step 1 - Enable the Linux development environment

1. Click on the Chromebook launcher.

2. Search for and open settings.

3. Search for and open the Developers options.

    *Developer options are found in different locations. On some Chromebooks they are found under Advanced options. On others they are found under About ChromeOS.*
    
4. Next to "Linux development environment," select Set up. 

5. Follow the wizard instructions.
    - You will be given a default username based on your email.
    - Use the recommended disk size.
    - The installation process can take a few minutes to complete.

6. A terminal window opens. 

7. Make sure everything is up to date by running this command: `sudo apt update && sudo apt upgrade -y`

8. Install gnome-keyring by running this command: `sudo apt install gnome-keyring  -y`

    > **gnome-keyring** is a recommended dependency of VS Code. It is a program that stores passwords for other programs.

9. Get your architecture by running this command: `arch` 
    - **x86_64** will require the .deb VS Code installation files.
    - **arm64** will require the .arm VS Code installation files.

## Step 2 - Install Visual Studio Code

1. Open a browser and search for VS Code. *https://code.visualstudio.com/*

2. Download
 the correct installation package for your architecture. 

    *The vs code website will recognize your device as a Chromebook and offer .deb and .arm installation packages.*

3. Go to the downlowads folder and find the installation package.

4. Right-click and choose install with Linux.

5. Click **OK** when prompted and wait for the installation to finish.

6. Go to the Chromebook launcher and search for VS Code.

7. Launch VS Code.

## Step 3 - (Optional) Optimize performance

### Enable memory swapping

1.  Press `Ctrl + Alt + T` to bring up Crosh.

    > **Crosh, or Chrome Shell**, is a Command Shell environment that is provided with ChromeOS.

2. Run the command swap enable with the amount of swap storage you want. For example, `swap enable 4000` creates 4GB of swap storage.

3. Reboot your device.

    > **swap enable** takes regular storage and allows you to use it for RAM. You can get rid of it by running the command `swap disable`, then restarting the device.

### Disable Android Apps

1. Open settings and search for "remove Google Play store."
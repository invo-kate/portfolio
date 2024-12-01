# How to install Visual Studio Code on a Chromebook

## Step 1 - Enable the Linux development environment

1. Open the Chromebook Launcher.

2. Open **Settings**.

3. In settings, search for and open **Developers options**.
  
4. Next to **Linux development environment**, select **Set up**. 

5. Follow the wizard instructions.
    - You will be given a default username based on your email.
    - Use the recommended disk size.
    - The installation process can take a few minutes to complete.

6. A terminal window will open. 

7. Make sure everything is up to date by running this command: `sudo apt update && sudo apt upgrade -y`

8. Install gnome-keyring by running this command: `sudo apt install gnome-keyring  -y`

    > Gnome Keyring is a recommended dependency of VS Code. Essentially, it is a program that stores security credentials for other programs.

9. Run this command: `arch`. Make note of your system architecture. 
    - **x86_64** will require the .deb VS Code installation files.
    - **arm64** will require the .arm VS Code installation files.

## Step 2 - Install Visual Studio Code

1. Open a browser and navigate to *https://code.visualstudio.com*

2. Download the correct installation package for your architecture. 

    > The Visual Studio Code website will recognize your device as a Chromebook and offer .deb and .arm installation packages.

3. Go to the downlowads folder and find the installation package.

4. Right-click and choose install with Linux.

5. Click **OK** when prompted and wait for the installation to finish.

6. Open the Chromebook Launcher and search for **Visual Studio Code**. It will be in a folder called **Linux apps** along with the Linux terminal.

7. Launch Visual Studio Code.

## Step 3 - (Optional) Optimize performance

### Enable memory swapping

1.  Press `Ctrl + Alt + T` to bring up Crosh.

    > Crosh, or Chrome Shell, is a Command Shell environment that is provided with ChromeOS.

2. Run the command swap enable with the amount of swap storage you want. For example, `swap enable 4000` creates 4GB of swap storage.

3. Restart your device.

    > `swap enable` takes regular storage and allows you to use it for RAM. You can get rid of it by running the command `swap disable`, then restarting the device.

### Disable Android apps

The Google Play store uses additional resources to download and manage Android apps on a Chromebook. Removing it can free up RAM and improve performance. You can reenable it at any time.

1. Open **Settings** and search for "remove Google Play store."

2. Click **Remove**.

3. A dialog box will open to inform you that disabling the any apps you have downloaded from the Google Play store will be delted.

4. Click **Remove Android apps**.

5. Restart your device.

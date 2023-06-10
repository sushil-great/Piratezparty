# How to Connect the KeePassXC Password Manager to LibreWolf in Linux?

> Credit : https://t.me/LinuxTechIndex

LibreWolf is NOT one of the browser options in [KeePassXC](https://t.me/LinuxTechIndex/588), so you need to add it's connection manually.

1.  Create a .mozilla folder in your home folder if it doesn't exist.

    `mkdir ~/.mozilla`

2.  Open [KeePassXC](https://t.me/LinuxTechIndex/588), and go to

    ```
    Tools
      ->Setting
        ->Browser Integration
    ```

3.  Check the "Firefox" checkbox

4.  Click "OK" button. This creates this file

    `org.keepassxc.keepassxc_browser.json`

    in this folder

    `~/.mozilla/native-messaging-hosts`

5.  Create the native-messaging-hosts folder inside the .librewolf folder in your home folder.

    `mkdir -p ~/.librewolf/native-messaging-hosts/`

6.  Copy the org.keepassxc.keepassxc_browser.json file from the .mozilla folder to the .librewolf folder

    `cp ~/.mozilla/native-messaging-hosts/org.keepassxc.keepassxc_browser.json ~/.librewolf/native-messaging-hosts/`

7.  Open LibreWolf, and follow these instructions for setting up KeePassXC in LibreWolf
    https://keepassxc.org/docs/KeePassXC_GettingStarted.html#_setup_browser_integration

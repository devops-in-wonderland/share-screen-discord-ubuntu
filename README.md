# Unable to Share Screen in Discord on Ubuntu

This repository is for Ubuntu users who are unable to share their screens in Discord.

---

## Description

This repository contains steps and solutions for Ubuntu users facing issues with screen sharing in Discord.

---

## Solution Steps

1. Open the terminal and enter the following command:

   ```bash
   echo $XDG_SESSION_TYPE

This command will display the session type.

2. If the output is "wayland," follow these steps:

   ```bash
   sudo vi /etc/gdm3/custom.conf
Enter this command to access the config file.

3. Inside the config file, if 'WaylandEnable' is commented out in the lines, uncomment it and set WaylandEnable=false.
4. Save and exit the file using 'esc :wq' command
5. Finally, restart your computer using the following command:
    ```bash
   sudo reboot now


ISSUE RESOLVED :partying_face:

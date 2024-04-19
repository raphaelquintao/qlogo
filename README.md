# QLogo
A Minimalist Plymouth Theme 

## Installation
1. Download files from [this link](https://github.com/raphaelquintao/qlogo/archive/refs/heads/master.zip).
2. Extract file: `unzip qlogo-master.zip`
3. Install Theme
   - Create target dir: `mkdir /usr/share/plymouth/themes/qlogo`
   - Copy files: `cp qlogo-master/* /usr/share/plymouth/themes/qlogo/`
5. Enable Theme
    - Debian based: `sudo plymouth-set-default-theme qlogo -R`

## Personalization
1. Change the `logo.png` to any logo you want.
2. Change the constans in `qlogo.script`
   ```C
   LOGO_HEIGHT = 150;  // Change the logo height.
   DOTS = 5;           // Change the amount of dot to show.
   SHOW_PROGRESS = 0;  // Show progress bar.
   FADE_OUT_DOTS = 1;  // Fade out the dots in animation.
   SHOW_MODE_TEXT = 1; // Enable or disable all boot status mode text.
   SHOW_MESSAGES = 1;  // Show the boot messsages as you can see on the second video.

   /* Here you can personalize the message and the color as you want. Maybe you wanna translate to your language.
    *
    * Position 1: Messsage
    * Position 2: Color in RGB
    * Position 3: 1 - Enable, 2 - Disabled
    */
   MODES["boot"] = ["Booting", [255, 255, 255], 1];
   MODES["shutdown"] = ["Shutting Down", [255, 255, 255], 1];
   MODES["reboot"] = ["Rebooting", [255, 255, 255], 1];
   MODES["updates"] = ["Updating...\nDon't turn off your computer", [255, 255, 255], 1];
   MODES["system-upgrade"] = ["System Upgrading...\nDon't turn off your computer", [255, 255, 255], 1];
   MODES["firmware-upgrade"] = ["Firmware Upgrading...\nDon't turn off your computer", [255, 255, 255], 1];
   MODES["system-reset"] = ["System Reseting", [255, 255, 255], 1];
   ```

## Preview
https://github.com/raphaelquintao/qlogo/assets/2568375/50d60eca-0c1b-4339-9f4c-8b002dc9288a

https://github.com/raphaelquintao/qlogo/assets/2568375/f010df72-a79a-4590-95a7-a13967cd4fc6


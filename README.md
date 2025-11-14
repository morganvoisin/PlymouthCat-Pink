# PlymouthCat-Pink
This is a Pink Plymouth theme.

[![Video](https://4.bp.blogspot.com/-gG0MBGjEE9M/WBYXrOGrVGI/AAAAAAAABVE/auGpLRYf7jor4hu3jurYGcjaVBapHyAVACLcB/s320/8998adc40112985a8f29cf414925d390.gif)](https://www.youtube.com/watch?v=c6f478VBhtE)


[Video] https://www.youtube.com/watch?v=c6f478VBhtE

For custom color, please let me know and I'll do an update to the files for you. Please reference the original creator's README to see instructions on how to get this on alternative distros (https://github.com/krishnan793/PlymouthTheme-Cat/blob/master/README.md)

# ------------------ ARCH LINUX DISTROS ------------------

## 1. Install Plymouth
Arch does not include Plymouth by default. Install it with:
    sudo pacman -Syu
    sudo pacman -S Plymouth

If you are using CachyOS, Plymouth may already be installed.


## 2. Clone this repo to your ~/.Downloads folder
    sudo git clone https://github.com/morganvoisin/PlymouthCat-Pink.git


## 3. Move the theme into your Plymouth theme folder (/usr/share/plymouth/themes)
    sudo cp -r <your-theme-folder> /usr/share/plymouth/themes/

Example:
    sudo cp -r ~/Downloads/PlymouthCat-Pink /usr/share/plymouth/themes/


## 4. Set the Theme using Plymouth theme selector:
    sudo plymouth-set-default-theme -R PlymouthCat-Pink

The `-R` flag automatically rebuilds your initramfs.

If you want to do it manually:
    sudo plymouth-set-default-theme PlymouthCat-Pink
    sudo mkinitcpio -P


## 5. Enable Plymouth at Boot
### GRUB Users
Edit `/etc/default/grub`:
    sudo nano /etc/default/grub

Find this line:
    GRUB_CMDLINE_LINUX_DEFAULT="loglevel=3 quiet"

Replace or add:
    GRUß_CMDLINE_LINUX_DEFAULT="quiet splash"

Save and update GRUB:
    sudo grub-mkconfig -o /boot/grub/grub.cfg


## 6. Reboot to See the Theme
    sudo reboot

You should now see your pink cat Plymouth animation at boot.


## Optional Tips
### Test the theme without rebooting
    sudo plymouthd

### Uninstall
    sudo rm -r /usr/share/plymouth/themes/PlymouthCat-Pink
    
(<img width="800" height="600" alt="progress-0" src="https://github.com/user-attachments/assets/87c813c4-cfea-4deb-8eaf-f7f3b6331ee1" />
























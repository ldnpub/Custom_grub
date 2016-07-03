# Custom_grub
Config file for booting ISO's directly from the hard drive.

This is a custom grub configuration that allows me to boot directly from ISO's on my hard drive on "Live CD mode". I give this on GitHub since i couldn't find the specifics for TAILS os.

I have 2 systems on my drive. A Windows 10 and Ubuntu 16.04 installed. And i also have 3 ISO's on a specific folder that i need to specify on the grub config file to boot on them.

This is my drives configuration:

└─ $ ▶lsblk -f
NAME   FSTYPE   LABEL      MOUNTPOINT
sda                                                        
├─sda1 ntfs     win                        
├─sda2 ntfs                                
├─sda3                                                     
├─sda4 swap            
├─sda5 ext4                /
├─sda6 ext4                /home
└─sda7 vfat                /media/data

From that you can edit your:

/etc/grub.d/40_custom

with your favorite text editor.

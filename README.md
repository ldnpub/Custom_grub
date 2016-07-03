# Custom_grub
Config file for booting ISO's directly from the hard drive.

This is a custom grub configuration that allows me to boot directly from ISO's on my hard drive on "Live CD mode". I give this on GitHub since i couldn't find the specifics for TAILS os.

I have 2 systems on my drive. A Windows 10 and Ubuntu 16.04 installed. And i also have 3 ISO's on a specific folder that i need to specify on the grub config file to boot on them.

This is my drives configuration:

└─ $ ▶lsblk -f
NAME   FSTYPE   LABEL UUID                                 MOUNTPOINT
sda                                                        
├─sda1 ntfs     win   08E4BA7A351E428A                     
├─sda2 ntfs           24747B9F747B7282                     
├─sda3                                                     
├─sda4 swap           a5f84c1f-0e0f-47ca-acb7-000467d1c02f 
├─sda5 ext4           bfa01813-c58d-4368-808e-c1a0a3f57078 /
├─sda6 ext4           eb37d2a1-4c71-4124-923d-fe00db52990b /home
└─sda7 vfat           5462-641B                            /media/data
loop0  squashfs                                            /snap/ubuntu-core/109
loop1  squashfs                                            /snap/htop/5

From that you can edit your:

/etc/grub.d/40_custom

with your favorite text editor.

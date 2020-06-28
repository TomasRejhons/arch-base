
                       -`
                      .o+`
                     `ooo/
                    `+oooo:
                   `+oooooo:
                   -+oooooo+:
                 `/:-:++oooo+:
                `/++++/+++++++:
               `/++++++++++++++:
              `/+++ooooooooooooo/`
             ./ooosssso++osssssso+`
            .oossssso-````/ossssss+`
           -osssssso.      :ssssssso.
          :osssssss/        osssso+++.
         /ossssssss/        +ssssooo/-
       `/ossssso+/:-        -:/+osssso+-
      `+sso+:-`                 `.-/+oso:
     `++:.                           `-/+/
     .`                                 `



# Minimalist Arch Linux Installation Script

Collection of very simple scripts I'm using to automate Arch installation (the whole installation process takes < 10 minutes). The script only supports EFI system. You can choose between ext4 and btrfs (both setups support system encryption). Swap is enabled via systemd-swap.

Learn the manual installation process first! https://wiki.archlinux.org/index.php/installation_guide

Do a few dry runs on a virtual machine!

- Boot Arch ISO
- Run <code>bash wget tomasrejhons.github.io/malis</code>
- Run <code>bash wget tomasrejhons.github.io/malis/config</code>
- Examine and edit malis config (Edit the drive you want to install the system on and mirror servers location etc)
- Run <code>bash malis</code>
- Examine and edit post-install (Edit the user name)
- Run <code>bash post-install</code>
- exit the root prompt, <code>umount -a</code> and <code>reboot</code>
- If you chose to use BTRFS, you can use snapper-setup to setup snapper and to create the initial system snapshot
- You can use install-desktop to install desktop environment (I'm currently using Gnome and AwesomeWM)
- (Optional) Run <code>sh archdi</code> to install additional software

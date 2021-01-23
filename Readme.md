
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

Collection of very simple scripts I'm using to automate Arch installation (the whole installation process takes < 10 minutes). The script only supports EFI system. The system is using BTRFS with encryption. Swap is enabled via systemd-swap.

Learn the manual installation process first! https://wiki.archlinux.org/index.php/installation_guide

Do a few dry runs on a virtual machine!

- Boot Arch ISO
- Run <code>curl -LJO tomasrejhons.github.io/malis</code>
- Run <code>curl -LJO tomasrejhons.github.io/malis/config</code>
- Examine and edit malis config (Edit the drive you want to install the system on and mirror servers location etc)
- Run <code>bash malis</code>
- Examine and edit post-install (Edit the user name)
- Run <code>bash post-install</code>
- exit the root prompt, <code>umount -a</code> and <code>reboot</code>
- You can use snapper-setup to setup snapper and to create the initial system snapshot
- (Optional) Run <code>sh archdi</code> to install additional software

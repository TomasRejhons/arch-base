
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

Collection of very simple scripts I'm using to automate Arch installation (the whole installation process takes < 10 minutes). The script is hardcoded for UEFI and BTRFS + snapper.

Learn the manual installation process first! https://wiki.archlinux.org/index.php/installation_guide

Do a few dry runs on a virtual machine!

- Boot Arch ISO
- Run <code>bash wget tomasrejhons.github.io/malis</code>
- Examine and edit malis (Edit the drive you want to install the system on and mirror servers location)
- Run <code>sh malis</code>
- Examine and edit malis-post-install (Edit the user name)
- Run <code>sh malis-post-install</code>
- exit the root prompt, <code>umount -a</code> and <code>reboot</code>
- Examine and edit malis-snapper
- Run <code>sh malis-snapper</code> to setup snapper and to create the initial system snapshot
- (Optional) Run <code>sh archdi</code> to install additional software


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



# Arch Linux Installation Script

Collection of very simple scripts I'm using to automate Arch installation (the whole installation process takes < 10 minutes). The script is hardcoded for UEFI and BTRFS + snapper.

Read through the manual installation process first! https://wiki.archlinux.org/index.php/installation_guide

Do a few dry runs on a virtual machine first!

- Boot Arch ISO
- Run <code>bash wget tomasrejhons.github.io/arch-baseinstall</code>
- Examine and edit arch-baseinstall (Edit the drive you want to install the system on and mirror servers location)
- Run <code>sh arch-baseinstall</code>
- Examine and edit arch-baseconfig (Edit the user name)
- Run <code>sh arch-baseconfig</code>
- exit the root prompt, <code>umount -a</code> and <code>reboot</code>
- Examine and edit arch-snapperconfig
- Run <code>sh arch-snapperconfig</code> to setup snapper and to create the initial system snapshot
- (Optional) Run <code>sh archdi</code> to install additional software

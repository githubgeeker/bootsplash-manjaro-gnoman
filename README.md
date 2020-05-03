# Bootsplash-manjaro-gnoman

Bootsplash theme for manjaro Linux with Gnome logo.

This project was based on multiple other great projects like:

https://github.com/Blacksuan19/Bootsplash-Themes

https://github.com/GrayJack/manjaro-grayjack/tree/master/PKGBUILDs/manjaro-bootsplash-green


Author: Pablo Lenna

# Installation:

- `git clone https://github.com/githubgeeker/bootsplash-manjaro-gnoman`
- `cd bootsplash-manjaro-noman`
- run `chmod +x bootsplash-manjaro-gnoman.sh`
- run `chmod +x bootsplash-packer`
- run `sh bootsplash-manjaro-gnoman.sh` to generate STL model.
- run `makepkg -s` to create an Arch package and install it with `pacman -U $package_name`or alternatively make and install with one single command: `makepkg -sci`
- append `bootsplash-manjaro-gnoman` hook at the end of HOOKS string in `/etc/mkinitcpio.conf`
- add `bootsplash.bootfile=bootsplash-themes/manjaro-gnoman/bootsplash` at the end of `GRUB_CMDLINE_LINUX` string in `/etc/default/grub` and don't forget to remove the `quiet` parameter!
- run `sudo mkinitcpio -P linux`
- run `sudo update-grub`

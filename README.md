## mank (MANange Kernel)
### About
Mank is a script used to manager installed kernels. It can be used to gather information on currently installed Linux kernels, initial RAM filesystems, kernel headers and bootloader entries and remove them. 

### Common commands
* `mank -h` Show mank manpage with more commands and examples
* `mank -la` List all installed kernels, kernel headers, initramfs files and bootloader entries
* `mank -r 5.7.8` Remove kernel, kernel headers, initramfs files and bootloader entries for the following kernel
* `mank -r 5.7.8 --dry` Do a dry run, prints list of files which will be removed during a non-dry run

## To-do
- [x] Basic functionality (List information, remove everything)
- [x] Separate remove functionality for every listable piece of information
- [ ] Optional configuration file (For custom filepaths and filenames etc..)
- [ ] Optional manual linking of kernel, bootloader entries, initramfs etc.. via "tracking file"
- [ ] Check if bootloader is GRUB or Systemd-boot, check if entry matches by checking 'linux' target on Systemd-boot

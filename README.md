# Bootsplash-Pine
Kernel Bootsplash theme for Manjaro patched Linux kernels using Pine logo

## Installation
1. Add `bootsplash-pine` to the end of the HOOKS section in your mkinitcpio.conf
2. Build and install package (It should automatically rebuild your initcpio)
3. Add `bootsplash.bootfile=bootsplash-themes/pine/bootsplash` to your kernel cmdline as well as other needed arguments such as `quiet`, likely through extlinux
4. Reboot

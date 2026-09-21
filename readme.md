# arch-live-usb
> single grub config file    
> [grub.cfg](./grub.cfg)    

```shell
#parted usb

#install grub for bios boot, (try to wipefs -a or dd if=/dev/zero, if errors occur)
#if not mbr, gpt table needs 1Mib partition which set bios_grub flag
grub-install --target=i386-pc --boot-directory=$boot $device

#install grub for uefi boot
grub-install --target=x86_64-efi --efi-directory=$esp --boot-directory=$boot --removable $device

#cp isofile into $esp/iso

#edit grub.cfg and check out carefully
#cp grub.cfg into $boot/grub
```

# grub-theme
> [condexpr01/grub-config-miku](https://github.com/condexpr01/grub-config-miku)    

# for-what
> Using usb install linux;    
> Nuke the entire system (write initramfs);    
> Nuke all storage devices which be plug in (write initramfs);    
> etc.    

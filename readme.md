# arch-live-usb
> single grub config file    
> [grub.cfg](./grub.cfg)    

```shell
#parted usb

#install grub
grub-install --target=x86_64-efi --efi-directory=$esp --boot-directory=$boot --removable

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

# Install Virtmanager on Arch Linux

# Update/Upgrade System
```bash
sudo pacman -Syyu
```

## Install virt-manager + dependencies
```bash
sudo pacman -S virt-manager qemu libvirt dmidecode ebtables
```

## Add group to your user
```bash
su -; usermod -aG libvirt "YOUR_USER" ; exit 
```

## Enable the service and check if it's running
```bash
sudo systemctl --now enable libvirtd
sudo systemctl status libvirtd
```


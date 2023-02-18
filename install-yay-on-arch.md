# Install yay on Arch Linux

## Install dependencies
```bash
sudo pacman -S binutils make gcc pkg-config fakeroot
```

## Clone the Repo
```
git clone https://aur.archlinux.org/yay.git /tmp/yay
cd /tmp/yay
```

## Build the package
```bash
makepkg -si
```

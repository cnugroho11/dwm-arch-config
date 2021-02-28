# DWM config

This is my DWM config i usually use. 

## Dependencies

Arch
```bash
pacman -S xorg xorg-xinit
```

## Installation

```bash
git clone https://github.com/cnugroho11/dwm-arch-config.git
cd dwm-arch-config
sudo make clean install
```

## Usage

Customization
```bash
cd dwm-arch-config
vim config.def.h
cp config.def.h config.h # you maybe need run this with sudo
sudo make clean install
```

Put this on your .xinitrc 
```bash

# put this if you want to loop dwm
while true; do
   dwm >/dev/null 2>&1
done

# run DWM
exec dwm
```


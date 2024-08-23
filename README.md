# deponejo

This is an Arch Linux repository to install zfs and some dracut hooks for pacman. The zfs package only supports building kernel modules with dkms. Also mkinitcpio is not supported.

## Usage
Add the following to `/etc/pacman.conf`:
```
[deponejo]
Server = https://raw.githubusercontent.com/SoongNoonien/deponejo/master
```

Run the following commands to add the key:
```bash
wget https://raw.githubusercontent.com/SoongNoonien/deponejo/master/public-key.asc
pacman-key -a public-key.asc
pacman-key --lsign-key 56DC9F466254CAB62C8CBFFA6D987150A72D19D0
rm public-key.asc
```

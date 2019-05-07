# refind-config-ubuntu
My refind config dual boot windows and ubuntu

My configuration have some configs:
- Boot directly into ubuntu, not showing grub menu
- Set timeout to 3 seconds, after that, boot into default entry
- Set default entry is the first entry

Step 1: Install refind boot loader
```
$ sudo apt-add-repository ppa:rodsmith/refind
$ sudo apt-get update
$ sudo apt-get install refind
```

Step 2: Download my refind config file:
```
wget -P ~/Downloads/ https://raw.githubusercontent.com/hoaibang07/refind-config-ubuntu/master/refind.conf
```

Step 3: Copy the file override the default config file:
```
sudo cp -f ~/Downloads/refind.conf /boot/efi/EFI/refind/refind.conf
```

# Ubunteira

A packer script to generate an Ubuntu minimal virtual machine.  
It uses the virtual version of the kernel.

Currently supports only the generation of VMWare Fusion images.

## Instructions

Rename the `packer.json.sample` file to `packer.json` and change the variables section with your settings.  
Then rename the `trusty_preseed.cfg.sample` file to `trusty_preseed.cfg` and change the user settings with the desired full name, username and password.

Run `packer build packer.json` to generate the image.

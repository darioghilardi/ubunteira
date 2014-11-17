# Ubunteira

A packer script to generate an Ubuntu minimal virtual machine.  
It uses the virtual version of the kernel.

Currently supports only the generation of VMWare Fusion images.

## Instructions

Rename the `packer.json.sample` file to `packer.json` and change the variables section with your settings.  
Then rename the `trusty_preseed.cfg.sample` file to `trusty_preseed.cfg` and change the user settings with the desired full name, username and password.

Run `packer build packer.json` to generate the image.

When the Ubuntu Server installation prompt ask you to select a language to continue the installation, exit from the prompt to permit to packer to continue the automated installation with the final vmware image creation. Otherwise, at the end of the installation, vmware loses the ssh connection and is not able to create the virtual machine files and you need to repeat the installation process.

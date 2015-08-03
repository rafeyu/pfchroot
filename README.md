# pfchroot - Prepare For Chroot

Doing `chroot` from my other distro again and again is boring. So .. I create this stuff to simplify `mount` actions before `chroot`ing.

**Remember!** This stuff is really useful if you do `pfchroot` from your other partitions (e.g you use dual boot system with other distros). Err ... it is doesn't means that `pfchroot` from live cd/usb is s&#42;ck, but because you have to install it again and again through your live cd/usb, unless it is already installed.

## Installing

Download with git:

    $ git clone https://github.com/rafeyu/pfchroot.git

Download with wget:

    $ wget https://raw.githubusercontent.com/rafeyu/pfchroot/master/pfchroot

Download with curl:

    $ curl -O https://raw.githubusercontent.com/rafeyu/pfchroot/master/pfchroot

Download with aria2:

    $ aria2c https://raw.githubusercontent.com/rafeyu/pfchroot/master/pfchroot

Then `chmod` it and go on!

## Usage

Please provide, at least, `--root` or `-r` to be mounted.

Example:

    # pfchroot --dir /mnt/mydir --root /dev/sda2 --boot /dev/sda1 --home /dev/sda3

or

    # pfchroot -d /mnt/mydir -r /dev/sda2 -b /dev/sda1 -m /dev/sda3

Thanks!

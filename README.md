# debian-installer
  Preseed dosyasını debian-installer menusune eklemek için menüye aşağıdaki satırları eklemek gerekir
label preseed
        menu label ^Preseed install
        kenrel debian-installer/amd64/linux
        append auto=true locale=tr_TR console-setup/charmap=UTF-8 console-keymaps-at/keymap=tr console-setup/layoutcode=tr console-setup/ask_detect=false pkgsel/language-pack-patterns=pkgsel/install-language-support=false interface=enp0s3 hostname=hostname01 domain="" url=tftp://192.168.56.50/stretch.cfg DEBCONF_DEBUG=5 initrd=debian-installer/amd64/initrd.gz ---quiet

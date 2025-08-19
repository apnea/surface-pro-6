# surface-pro-6
install linux on surface pro 6

- install cachos via usb
  - issue: with the high pixel density neither adjusting scale nor resolution improves installer ui components
  - issue: wifi widget does not start wifi
    - resolution: use ```nmtui``` from the shell
- post-install
  - issue: wifi hw not recognised
    - resolution: ```nmcli general``` and ```inxi -N```, latter shows Marvell wifi card. Download https://archlinux.org/packages/core/any/linux-firmware-marvell/ onto usb stick and install
  - issue: bluetooth hw not recognised
    - resolution: bluetooth hw on Marvell card, fixed by previous step
- https://github.com/linux-surface/linux-surface/wiki/Installation-and-Setup
  - turns out surface kernel is recent but trails cachyos by a few months
  - fixes touch screen
- libcamera et al
  - fixes camera

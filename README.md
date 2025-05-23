# Andy's Custom VanillaOS image

## Changes

- GitHub workflows will build multiple different containers with my additions (desktop and nvidia images as of writing, [matrix](https://github.com/andrew-stclair/Custom-VanillaOS/blob/0790409e83fda3ae7ecafa6b8a22c0293c5090f7/.github/workflows/vib-build.yml#L18-L24) and [yaml updater](https://github.com/andrew-stclair/Custom-VanillaOS/blob/0790409e83fda3ae7ecafa6b8a22c0293c5090f7/.github/workflows/vib-build.yml#L32-L37) for reference)
- Installing Solaar to manage logitech devices.
- Installing syncthing for synchronising my files between my devices.
- Installing scdaemon to use hardware gpg cards.
- Installing a bunch of udev rules to allow me to use SDR's, the CH341A chip reader, and steam related hardware.

# Grub Boot GIF
Set a GIF for Grub boot (like windows logo on startup).

## Install

```sh
git clone https://github.com/MysticalMike60t/grubbootgif.git
cd grubbootgif
sudo install -m755 set-boot-gif /usr/local/bin/
```

## Usage

You do need to use `sudo` before any usage of `set-boot-gif`, since it modifies using **Plymouth**, which needs sudo privileges too.

### Play GIF Once, Stay on last frame

```sh
sudo set-boot-gif GIF_FILE_PATH
```

### Loop GIF until finish booting

```sh
sudo set-boot-gif -l GIF_FILE_PATH
```

### Specify GIF Height and Framerate

```sh
sudo set-boot-gif -H 1440 -f 15 GIF_FILE_PATH
```

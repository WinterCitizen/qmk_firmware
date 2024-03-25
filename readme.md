## Installation
Fork the repo

Setup qmk on your machine
```bash
sudo pacman -S qmk
qmk setup <your_github_username>/qmk_firmware
```

Perform the next action first with one side of the keyboard connected to USB and then with the other.
It will ask you to press reset button at some point. It's located near the side of your keyboard between TRRS jack and pro micro controller.
```bash
qmk flash -kb crkbd/rev1 -km custom
```

`crkbd/rev1` directory is a path relative to `<path_to_cloned_qmk_firmware>/keyboards` and `custom` is a keymap directory located in `<path_to_cloned_qmk_firmware>/keyboards/crkbd` directory.

After that you should be good to go. Create your own keymap directory in the corresponding keyboard directory or just use `custom` and change `keymap.c` file.

PS Vita homebrew for remapping controls.

## Features

* Remap any button, sticks (4 directions), back touchscreen (4 virtual buttons)
* Remap single button to button combination
* Configure front and back touchscreen, left and right stick deadzones
* GUI

## Troubleshoot
* Plugin doesn't work:
  * Pirated games not supported
  * If the notice message doesn't appear in the game: make sure that you've edited taiHEN's `config.txt` and reloaded it trough `molecularShell`
  * Other way the game may be unsupported

* Config not saved
  * Make sure that you've added at least 1 button

## License
GPLv3

## Build
1. Build taiHEN plugin (in `plugin` directory `mkdir build && cd build && cmake .. && make`)
1. Update `CONFIG_MEM_OFFSET` in `src/remap/config.h` to the offset generated by `make addr` command in `plugin/build` folder
1. Build the homebrew (in root folder `mkdir build && cd build && cmake .. && make`)

## Credits
Project use source code from following repositories:

* [VitaShell][]
* [vita-savemgr][]
* [rinCheat][]

Special thanks to #vitasdk and Scorpeg's [ButtonSwap](https://github.com/Scorpeg/Button-Swap)

[VitaShell]: https://github.com/TheOfficialFloW/VitaShell
[vita-savemgr]: https://github.com/d3m3vilurr/vita-savemgr
[rinCheat]: https://github.com/Rinnegatamante/rinCheat
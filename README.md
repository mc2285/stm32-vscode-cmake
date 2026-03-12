# A template to use STM32CubeMX CMake projects with VSCode without CubeIDE extension pack

## Dependencies (Arch)

```bash
paru -S stm32cubemx # or whichever AUR helper you happen to have
# arm-none-eabi- gcc toolchain, openocd for flashing and clang to be able to use clangd
pacman -S arm-none-eabi-gcc arm-none-eabi-gdb arm-none-eabi-binutils arm-none-eabi-newlib openocd clang
```

Also, STM32CubeProg is recommended to get SVD file bundle; AUR is broken as of 2026.03.05
You might as well get the `.svd` files from wherever you like

## Workflow

1. `STM32CubeMX` -> Save project in this directory -> Configure cmake project using GCC toolchain -> export
2. Open `VSCode` -> `cmake: select configure preset` -> `Debug`
3. Press `F5` in `main.c`
4. You should be good to go

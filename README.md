# A template to use STM32CubeMX CMake projects with VSCode without CubeIDE extension pack

## Dependencies (Arch)
```bash
paru -S stm32cubemx # or whichever AUR helper you happen to have
pacman -S arm-none-eabi-gcc arm-none-eabi-gdb arm-none-eabi-binutils arm-none-eabi-newlib openocd
```

Also, STM32CubeProg from ST website is required; AUR is broken as of 2026.03.05

# runelf
Runs .elf or .hex executables in a screen, using the GNU Debugger for the ARM EABI target, without having to manually define your target, load and continue your program when your intentions are to simply rerun your updated project

Checks on whether or not a screen is already running are made. Additional checks and features such as a `kill` argument are welcome! The latter requires you to attach to the screen and ctrl-c is from there as of now.

This is additional to texane's stlink tools for linux: https://github.com/texane/stlink

## using runelf to reflash and run your program
Make sure `st-util` is running and `screen` is installed!
Either place runelf in `/usr/local/bin` or keep it in your current working directory

respectively;

```sh
runelf executable.elf
```

```sh
./runelf executable.elf
```

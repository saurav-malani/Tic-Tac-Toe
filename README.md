



## Command for compiling using GCC (GTK+ 3.0 Libraries must be installed first):
```
gcc -o TicTacToe main.c -Wall `pkg-config --cflags --libs gtk+-3.0` -export-dynamic
```
## Command on windows with MSYS (Keep all required DLL's in the folder with the executable):
```
gcc main.c -o TicTacToe.exe `pkg-config --cflags --libs gtk+-3.0` -Wl,--export-all-symbols -mwindows


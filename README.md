# system

## tools

### gcc
risc-v gcc `riscv64-unknown-elf-gcc`

1. complie to executable file
```
gcc app.c -o app
```
2. compile to assemble
```
gcc -S app.c -o app.s
```
3. optimization level
- -O0 no optimization, default option
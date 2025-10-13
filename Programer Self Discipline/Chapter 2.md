
## Complie 
- Prepressing - Compilation - Assembly - Linking
- Prepressing
    - gcc -E app.c -o app.i
    - handle `#include`, `define`, `#if` ect.
    - delete `define`, extract all definition
    - handle conditional instructions, `#if`, `#ifdef`
    - handle `@include`, include all content from files
    - delete all comments
    - add line no and filename flag for debug info
    - keep all `#pragma`
- Compilation
    - gcc -S app.i -o app.s
- Assembly
    - gcc -c app.s -o hello.o
- Linking
    - ld -static crtl.o crti.o crtbeginT.o hello.o -start-group -lgcc -lgcc_eh -lc-end-group crtend.o crtn.o
    - Relocate address, Organize sources
## Module Linking
- Communication between modules: function call, variable access
- Address and Storage Allocation, Symbol Resolution, Relocation

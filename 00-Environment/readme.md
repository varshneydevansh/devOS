*Concepts you may want to Google beforehand: linux, mac, terminal, compiler, emulator, nasm, qemu*

**Goal: Install the software required to run this tutorial**
## nasm
Compiling an assembly program with NASM can be done on Linux or Windows, as NASM is available for both platforms. 
Netwide Assembler (NASM) is an assembler and dissembler for the Intel x86 architecture and is commonly used to create 16-bit, 32-bit (IA-32), and 64-bit (x86-64) programs. 

An assemble will turn your low-level coding, using mnemonics, into machine language that can be understood by the processor. 

If you're running Debian or Ubuntu, simply type the command: 

```sh
$ sudo apt-get install nasm
```

If you have another Linux distribution, you must use your distribution's package manager (e.g. Urpmi, Yum, Emerge) or download NASM from the official site. 

Use the following command line to assemble your source file: 

```sh
nasm -f elf test.asm
```

## qemu
Just replace qemu with qemu-system-i386 or qemu-system-x86_64 as appropriate (whether you want a 32-bit or 64-bit system, and which ISO you're using).

You can also use aqemu, which is a graphical (GUI) front-end to qemu.
```sh
$ sudo apt-get install qemu-system
or
$ sudo apt-get install aqemu
```
example - 
```sh

 $ qemu-system-x86_64 boot_sect_simple.bin
```

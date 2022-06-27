```
#for i in `ls  | sed 's/bash-//g' ` ; do echo -e "## $i \n$ readelf -h bash-$i\n " ; readelf -h bash-$i ; echo "# file bash-$i" ; file bash-$i ; done
```


## aarch64 
```
$ readelf -h bash-aarch64
 
ELF Header:
  Magic:   7f 45 4c 46 02 01 01 00 00 00 00 00 00 00 00 00 
  Class:                             ELF64
  Data:                              2's complement, little endian
  Version:                           1 (current)
  OS/ABI:                            UNIX - System V
  ABI Version:                       0
  Type:                              DYN (Position-Independent Executable file)
  Machine:                           AArch64
  Version:                           0x1
  Entry point address:               0x30580
  Start of program headers:          64 (bytes into file)
  Start of section headers:          1431704 (bytes into file)
  Flags:                             0x0
  Size of this header:               64 (bytes)
  Size of program headers:           56 (bytes)
  Number of program headers:         11
  Size of section headers:           64 (bytes)
  Number of section headers:         31
  Section header string table index: 30
$ file bash-aarch64
bash-aarch64: ELF 64-bit LSB pie executable, ARM aarch64, version 1 (SYSV), dynamically linked, interpreter /lib/ld-linux-aarch64.so.1, BuildID[sha1]=01d99a5fd3fcf3cc4565d6ba4bf2748310bdacd4, for GNU/Linux 3.7.0, stripped
```
## alpha 
```
$ readelf -h bash-alpha
 
ELF Header:
  Magic:   7f 45 4c 46 02 01 01 00 00 00 00 00 00 00 00 00 
  Class:                             ELF64
  Data:                              2's complement, little endian
  Version:                           1 (current)
  OS/ABI:                            UNIX - System V
  ABI Version:                       0
  Type:                              EXEC (Executable file)
  Machine:                           Alpha
  Version:                           0x1
  Entry point address:               0x120018ec0
  Start of program headers:          64 (bytes into file)
  Start of section headers:          943944 (bytes into file)
  Flags:                             0x0
  Size of this header:               64 (bytes)
  Size of program headers:           56 (bytes)
  Number of program headers:         8
  Size of section headers:           64 (bytes)
  Number of section headers:         28
  Section header string table index: 27
$ file bash-alpha
bash-alpha: ELF 64-bit LSB executable, Alpha (unofficial), version 1 (SYSV), dynamically linked, interpreter /lib/ld-linux.so.2, for GNU/Linux 2.2.5, stripped
```
## armv5tel 
```
$ readelf -h bash-armv5tel
 
ELF Header:
  Magic:   7f 45 4c 46 01 01 01 00 00 00 00 00 00 00 00 00 
  Class:                             ELF32
  Data:                              2's complement, little endian
  Version:                           1 (current)
  OS/ABI:                            UNIX - System V
  ABI Version:                       0
  Type:                              EXEC (Executable file)
  Machine:                           ARM
  Version:                           0x1
  Entry point address:               0x1f1b8
  Start of program headers:          52 (bytes into file)
  Start of section headers:          760032 (bytes into file)
  Flags:                             0x5000002, Version5 EABI, <unknown>
  Size of this header:               52 (bytes)
  Size of program headers:           32 (bytes)
  Number of program headers:         8
  Size of section headers:           40 (bytes)
  Number of section headers:         29
  Section header string table index: 28
$ file bash-armv5tel
bash-armv5tel: ELF 32-bit LSB executable, ARM, EABI5 version 1 (SYSV), dynamically linked, interpreter /lib/ld-linux.so.3, for GNU/Linux 2.6.18, BuildID[sha1]=e23bf64080bba917cd80007daa680b7d7038b0e9, stripped
```
## armv7hl 
```
$ readelf -h bash-armv7hl
 
ELF Header:
  Magic:   7f 45 4c 46 01 01 01 00 00 00 00 00 00 00 00 00 
  Class:                             ELF32
  Data:                              2's complement, little endian
  Version:                           1 (current)
  OS/ABI:                            UNIX - System V
  ABI Version:                       0
  Type:                              DYN (Position-Independent Executable file)
  Machine:                           ARM
  Version:                           0x1
  Entry point address:               0x21840
  Start of program headers:          52 (bytes into file)
  Start of section headers:          1276060 (bytes into file)
  Flags:                             0x5000400, Version5 EABI, hard-float ABI
  Size of this header:               52 (bytes)
  Size of program headers:           32 (bytes)
  Number of program headers:         9
  Size of section headers:           40 (bytes)
  Number of section headers:         31
  Section header string table index: 30
$ file bash-armv7hl
bash-armv7hl: ELF 32-bit LSB pie executable, ARM, EABI5 version 1 (SYSV), dynamically linked, interpreter /lib/ld-linux-armhf.so.3, BuildID[sha1]=69658d3d2fea223d912f206893294ef0c601e570, for GNU/Linux 3.2.0, stripped
```
## hppa_debian 
```
$ readelf -h bash-hppa_debian
 
ELF Header:
  Magic:   7f 45 4c 46 01 02 01 03 00 00 00 00 00 00 00 00 
  Class:                             ELF32
  Data:                              2's complement, big endian
  Version:                           1 (current)
  OS/ABI:                            UNIX - GNU
  ABI Version:                       0
  Type:                              EXEC (Executable file)
  Machine:                           HPPA
  Version:                           0x1
  Entry point address:               0x32000
  Start of program headers:          52 (bytes into file)
  Start of section headers:          1170772 (bytes into file)
  Flags:                             0x210, PA-RISC 1.1
  Size of this header:               52 (bytes)
  Size of program headers:           32 (bytes)
  Number of program headers:         8
  Size of section headers:           40 (bytes)
  Number of section headers:         30
  Section header string table index: 29
$ file bash-hppa_debian
bash-hppa_debian: ELF 32-bit MSB executable, PA-RISC, 1.1 version 1 (GNU/Linux), dynamically linked, interpreter /lib/ld.so.1, BuildID[sha1]=933502bf56e13dfdd507627f8661bbb5f522eb05, for GNU/Linux 3.2.0, stripped
```
## i686 
```
$ readelf -h bash-i686
 
ELF Header:
  Magic:   7f 45 4c 46 01 01 01 00 00 00 00 00 00 00 00 00 
  Class:                             ELF32
  Data:                              2's complement, little endian
  Version:                           1 (current)
  OS/ABI:                            UNIX - System V
  ABI Version:                       0
  Type:                              DYN (Position-Independent Executable file)
  Machine:                           Intel 80386
  Version:                           0x1
  Entry point address:               0x22c40
  Start of program headers:          52 (bytes into file)
  Start of section headers:          1621744 (bytes into file)
  Flags:                             0x0
  Size of this header:               52 (bytes)
  Size of program headers:           32 (bytes)
  Number of program headers:         11
  Size of section headers:           40 (bytes)
  Number of section headers:         30
  Section header string table index: 29
$ file bash-i686
bash-i686: ELF 32-bit LSB pie executable, Intel 80386, version 1 (SYSV), dynamically linked, interpreter /lib/ld-linux.so.2, for GNU/Linux 3.2.0, BuildID[sha1]=df36bcabc1c5aeadc9aae791bb92fdcfe932d944, stripped, too many notes (256)
```
## ia64 
```
$ readelf -h bash-ia64
 
ELF Header:
  Magic:   7f 45 4c 46 02 01 01 00 00 00 00 00 00 00 00 00 
  Class:                             ELF64
  Data:                              2's complement, little endian
  Version:                           1 (current)
  OS/ABI:                            UNIX - System V
  ABI Version:                       0
  Type:                              EXEC (Executable file)
  Machine:                           Intel IA-64
  Version:                           0x1
  Entry point address:               0x400000000001f2a0
  Start of program headers:          64 (bytes into file)
  Start of section headers:          1500000 (bytes into file)
  Flags:                             0x10, 64-bit
  Size of this header:               64 (bytes)
  Size of program headers:           56 (bytes)
  Number of program headers:         8
  Size of section headers:           64 (bytes)
  Number of section headers:         32
  Section header string table index: 31
$ file bash-ia64
bash-ia64: ELF 64-bit LSB executable, IA-64, version 1 (SYSV), dynamically linked, interpreter /lib/ld-linux-ia64.so.2, for GNU/Linux 2.4.0, stripped
```
## m68k_debian 
```
$ readelf -h bash-m68k_debian
 
ELF Header:
  Magic:   7f 45 4c 46 01 02 01 00 00 00 00 00 00 00 00 00 
  Class:                             ELF32
  Data:                              2's complement, big endian
  Version:                           1 (current)
  OS/ABI:                            UNIX - System V
  ABI Version:                       0
  Type:                              EXEC (Executable file)
  Machine:                           MC68000
  Version:                           0x1
  Entry point address:               0x80021d7c
  Start of program headers:          52 (bytes into file)
  Start of section headers:          941676 (bytes into file)
  Flags:                             0x0
  Size of this header:               52 (bytes)
  Size of program headers:           32 (bytes)
  Number of program headers:         9
  Size of section headers:           40 (bytes)
  Number of section headers:         27
  Section header string table index: 26
$ file bash-m68k_debian
bash-m68k_debian: ELF 32-bit MSB executable, Motorola m68k, 68020, version 1 (SYSV), dynamically linked, interpreter /lib/ld.so.1, BuildID[sha1]=f3b7ea56cacab3e3609cff947e45f1862ca24355, for GNU/Linux 3.2.0, stripped
```
## mips64el-debian 
```
$ readelf -h bash-mips64el-debian
 
ELF Header:
  Magic:   7f 45 4c 46 02 01 01 00 00 00 00 00 00 00 00 00 
  Class:                             ELF64
  Data:                              2's complement, little endian
  Version:                           1 (current)
  OS/ABI:                            UNIX - System V
  ABI Version:                       0
  Type:                              EXEC (Executable file)
  Machine:                           MIPS R3000
  Version:                           0x1
  Entry point address:               0x120022280
  Start of program headers:          64 (bytes into file)
  Start of section headers:          1282552 (bytes into file)
  Flags:                             0x80000007, noreorder, pic, cpic, mips64r2
  Size of this header:               64 (bytes)
  Size of program headers:           56 (bytes)
  Number of program headers:         10
  Size of section headers:           64 (bytes)
  Number of section headers:         32
  Section header string table index: 31
$ file bash-mips64el-debian
bash-mips64el-debian: ELF 64-bit LSB executable, MIPS, MIPS64 rel2 version 1 (SYSV), dynamically linked, interpreter /lib64/ld.so.1, BuildID[sha1]=cf41f4208cda973f7dc8df7970861f52558f8578, for GNU/Linux 3.2.0, stripped
```
## mips-debian 
```
$ readelf -h bash-mips-debian
 
ELF Header:
  Magic:   7f 45 4c 46 01 02 01 00 00 00 00 00 00 00 00 00 
  Class:                             ELF32
  Data:                              2's complement, big endian
  Version:                           1 (current)
  OS/ABI:                            UNIX - System V
  ABI Version:                       0
  Type:                              EXEC (Executable file)
  Machine:                           MIPS R3000
  Version:                           0x1
  Entry point address:               0x41be20
  Start of program headers:          52 (bytes into file)
  Start of section headers:          1234004 (bytes into file)
  Flags:                             0x70001007, noreorder, pic, cpic, o32, mips32r2
  Size of this header:               52 (bytes)
  Size of program headers:           32 (bytes)
  Number of program headers:         12
  Size of section headers:           40 (bytes)
  Number of section headers:         34
  Section header string table index: 33
$ file bash-mips-debian
bash-mips-debian: ELF 32-bit MSB executable, MIPS, MIPS32 rel2 version 1 (SYSV), dynamically linked, interpreter /lib/ld.so.1, for GNU/Linux 3.2.0, BuildID[sha1]=cf04fe027c6d0ffdc84ca97b264d0c67f0132c15, stripped
```
## mipsel-debian 
```
$ readelf -h bash-mipsel-debian
 
ELF Header:
  Magic:   7f 45 4c 46 01 01 01 00 00 00 00 00 00 00 00 00 
  Class:                             ELF32
  Data:                              2's complement, little endian
  Version:                           1 (current)
  OS/ABI:                            UNIX - System V
  ABI Version:                       0
  Type:                              EXEC (Executable file)
  Machine:                           MIPS R3000
  Version:                           0x1
  Entry point address:               0x41be20
  Start of program headers:          52 (bytes into file)
  Start of section headers:          1234004 (bytes into file)
  Flags:                             0x70001007, noreorder, pic, cpic, o32, mips32r2
  Size of this header:               52 (bytes)
  Size of program headers:           32 (bytes)
  Number of program headers:         12
  Size of section headers:           40 (bytes)
  Number of section headers:         34
  Section header string table index: 33
$ file bash-mipsel-debian
bash-mipsel-debian: ELF 32-bit LSB executable, MIPS, MIPS32 rel2 version 1 (SYSV), dynamically linked, interpreter /lib/ld.so.1, for GNU/Linux 3.2.0, BuildID[sha1]=0de4fa415f908fd0eb0dd4980ddc11a8ee135dc6, stripped
```
## ppc 
```
$ readelf -h bash-ppc
 
ELF Header:
  Magic:   7f 45 4c 46 01 02 01 00 00 00 00 00 00 00 00 00 
  Class:                             ELF32
  Data:                              2's complement, big endian
  Version:                           1 (current)
  OS/ABI:                            UNIX - System V
  ABI Version:                       0
  Type:                              EXEC (Executable file)
  Machine:                           PowerPC
  Version:                           0x1
  Entry point address:               0x10017970
  Start of program headers:          52 (bytes into file)
  Start of section headers:          1067496 (bytes into file)
  Flags:                             0x0
  Size of this header:               52 (bytes)
  Size of program headers:           32 (bytes)
  Number of program headers:         9
  Size of section headers:           40 (bytes)
  Number of section headers:         31
  Section header string table index: 30
$ file bash-ppc
bash-ppc: ELF 32-bit MSB executable, PowerPC or cisco 4500, version 1 (SYSV), dynamically linked, interpreter /lib/ld.so.1, for GNU/Linux 2.6.32, BuildID[sha1]=13d0636253d89c267e473c77e8082ce9878f8c7d, stripped
```
## ppc64 
```
$ readelf -h bash-ppc64
 
ELF Header:
  Magic:   7f 45 4c 46 02 02 01 00 00 00 00 00 00 00 00 00 
  Class:                             ELF64
  Data:                              2's complement, big endian
  Version:                           1 (current)
  OS/ABI:                            UNIX - System V
  ABI Version:                       0
  Type:                              DYN (Position-Independent Executable file)
  Machine:                           PowerPC64
  Version:                           0x1
  Entry point address:               0x1861b8
  Start of program headers:          64 (bytes into file)
  Start of section headers:          1673536 (bytes into file)
  Flags:                             0x1, abiv1
  Size of this header:               64 (bytes)
  Size of program headers:           56 (bytes)
  Number of program headers:         9
  Size of section headers:           64 (bytes)
  Number of section headers:         30
  Section header string table index: 29
$ file bash-ppc64
bash-ppc64: ELF 64-bit MSB pie executable, 64-bit PowerPC or cisco 7500, Power ELF V1 ABI, version 1 (SYSV), dynamically linked, interpreter /lib64/ld64.so.1, for GNU/Linux 3.2.0, BuildID[sha1]=3e994fff7d5295daf7e1011d2c4eb9b6abba33d6, stripped, too many notes (256)
```
## ppc64le 
```
$ readelf -h bash-ppc64le
 
ELF Header:
  Magic:   7f 45 4c 46 02 01 01 00 00 00 00 00 00 00 00 00 
  Class:                             ELF64
  Data:                              2's complement, little endian
  Version:                           1 (current)
  OS/ABI:                            UNIX - System V
  ABI Version:                       0
  Type:                              DYN (Position-Independent Executable file)
  Machine:                           PowerPC64
  Version:                           0x1
  Entry point address:               0x31cd4
  Start of program headers:          64 (bytes into file)
  Start of section headers:          1824800 (bytes into file)
  Flags:                             0x2, abiv2
  Size of this header:               64 (bytes)
  Size of program headers:           56 (bytes)
  Number of program headers:         9
  Size of section headers:           64 (bytes)
  Number of section headers:         29
  Section header string table index: 28
$ file bash-ppc64le
bash-ppc64le: ELF 64-bit LSB pie executable, 64-bit PowerPC or cisco 7500, OpenPOWER ELF V2 ABI, version 1 (SYSV), dynamically linked, interpreter /lib64/ld64.so.2, BuildID[sha1]=d832ffa5881caf09914b55b067df75775bcefa29, for GNU/Linux 3.10.0, stripped
```
## riscv64_debian 
```
$ readelf -h bash-riscv64_debian
 
ELF Header:
  Magic:   7f 45 4c 46 02 01 01 00 00 00 00 00 00 00 00 00 
  Class:                             ELF64
  Data:                              2's complement, little endian
  Version:                           1 (current)
  OS/ABI:                            UNIX - System V
  ABI Version:                       0
  Type:                              DYN (Position-Independent Executable file)
  Machine:                           RISC-V
  Version:                           0x1
  Entry point address:               0x32f7c
  Start of program headers:          64 (bytes into file)
  Start of section headers:          932912 (bytes into file)
  Flags:                             0x5, RVC, double-float ABI
  Size of this header:               64 (bytes)
  Size of program headers:           56 (bytes)
  Number of program headers:         10
  Size of section headers:           64 (bytes)
  Number of section headers:         27
  Section header string table index: 26
$ file bash-riscv64_debian
bash-riscv64_debian: ELF 64-bit LSB pie executable, UCB RISC-V, RVC, double-float ABI, version 1 (SYSV), dynamically linked, interpreter /lib/ld-linux-riscv64-lp64d.so.1, BuildID[sha1]=76d8296819bcc14a97fa7627b96c1cd0092e2d96, for GNU/Linux 4.15.0, stripped
```
## s390 
```
$ readelf -h bash-s390
 
ELF Header:
  Magic:   7f 45 4c 46 01 02 01 00 00 00 00 00 00 00 00 00 
  Class:                             ELF32
  Data:                              2's complement, big endian
  Version:                           1 (current)
  OS/ABI:                            UNIX - System V
  ABI Version:                       0
  Type:                              DYN (Shared object file)
  Machine:                           IBM S/390
  Version:                           0x1
  Entry point address:               0x25800
  Start of program headers:          52 (bytes into file)
  Start of section headers:          1086096 (bytes into file)
  Flags:                             0x0
  Size of this header:               52 (bytes)
  Size of program headers:           32 (bytes)
  Number of program headers:         9
  Size of section headers:           40 (bytes)
  Number of section headers:         29
  Section header string table index: 28
$ file bash-s390
bash-s390: ELF 32-bit MSB shared object, IBM S/390, version 1 (SYSV), dynamically linked, interpreter /lib/ld.so.1, for GNU/Linux 2.6.32, BuildID[sha1]=7de248bf6bcdbeca7cc19a3b4e42478160e7ecb1, stripped
```
## s390x 
```
$ readelf -h bash-s390x
 
ELF Header:
  Magic:   7f 45 4c 46 02 02 01 00 00 00 00 00 00 00 00 00 
  Class:                             ELF64
  Data:                              2's complement, big endian
  Version:                           1 (current)
  OS/ABI:                            UNIX - System V
  ABI Version:                       0
  Type:                              DYN (Position-Independent Executable file)
  Machine:                           IBM S/390
  Version:                           0x1
  Entry point address:               0x311a0
  Start of program headers:          64 (bytes into file)
  Start of section headers:          1443808 (bytes into file)
  Flags:                             0x0
  Size of this header:               64 (bytes)
  Size of program headers:           56 (bytes)
  Number of program headers:         9
  Size of section headers:           64 (bytes)
  Number of section headers:         29
  Section header string table index: 28
$ file bash-s390x
bash-s390x: ELF 64-bit MSB pie executable, IBM S/390, version 1 (SYSV), dynamically linked, interpreter /lib/ld64.so.1, BuildID[sha1]=122e75e79626dc79e838b5f430b2db897024c082, for GNU/Linux 3.2.0, stripped
```
## sh4_debian 
```
$ readelf -h bash-sh4_debian
 
ELF Header:
  Magic:   7f 45 4c 46 01 01 01 00 00 00 00 00 00 00 00 00 
  Class:                             ELF32
  Data:                              2's complement, little endian
  Version:                           1 (current)
  OS/ABI:                            UNIX - System V
  ABI Version:                       0
  Type:                              EXEC (Executable file)
  Machine:                           Renesas / SuperH SH
  Version:                           0x1
  Entry point address:               0x422110
  Start of program headers:          52 (bytes into file)
  Start of section headers:          948556 (bytes into file)
  Flags:                             0x17, sh2a-or-sh4
  Size of this header:               52 (bytes)
  Size of program headers:           32 (bytes)
  Number of program headers:         10
  Size of section headers:           40 (bytes)
  Number of section headers:         27
  Section header string table index: 26
$ file bash-sh4_debian
bash-sh4_debian: ELF 32-bit LSB executable, Renesas SH, version 1 (SYSV), dynamically linked, interpreter /lib/ld-linux.so.2, BuildID[sha1]=6ce6f7983a6c760055b17bd73c57b4e4611ae51e, for GNU/Linux 3.2.0, stripped
```
## sparc64_sparcv9 
```
$ readelf -h bash-sparc64_sparcv9
 
ELF Header:
  Magic:   7f 45 4c 46 02 02 01 00 00 00 00 00 00 00 00 00 
  Class:                             ELF64
  Data:                              2's complement, big endian
  Version:                           1 (current)
  OS/ABI:                            UNIX - System V
  ABI Version:                       0
  Type:                              EXEC (Executable file)
  Machine:                           Sparc v9
  Version:                           0x1
  Entry point address:               0x11b260
  Start of program headers:          64 (bytes into file)
  Start of section headers:          933176 (bytes into file)
  Flags:                             0x2, rmo
  Size of this header:               64 (bytes)
  Size of program headers:           56 (bytes)
  Number of program headers:         8
  Size of section headers:           64 (bytes)
  Number of section headers:         27
  Section header string table index: 26
$ file bash-sparc64_sparcv9
bash-sparc64_sparcv9: ELF 64-bit MSB executable, SPARC V9, relaxed memory ordering, version 1 (SYSV), dynamically linked, interpreter /lib64/ld-linux.so.2, for GNU/Linux 2.6.18, BuildID[sha1]=aa5af4ae81ceadb617cfa74ee8778e5421674a03, stripped
```
## sparc_sparcv9 
```
$ readelf -h bash-sparc_sparcv9
 
ELF Header:
  Magic:   7f 45 4c 46 01 02 01 00 00 00 00 00 00 00 00 00 
  Class:                             ELF32
  Data:                              2's complement, big endian
  Version:                           1 (current)
  OS/ABI:                            UNIX - System V
  ABI Version:                       0
  Type:                              EXEC (Executable file)
  Machine:                           Sparc v8+
  Version:                           0x1
  Entry point address:               0x266a0
  Start of program headers:          52 (bytes into file)
  Start of section headers:          888956 (bytes into file)
  Flags:                             0x100
  Size of this header:               52 (bytes)
  Size of program headers:           32 (bytes)
  Number of program headers:         8
  Size of section headers:           40 (bytes)
  Number of section headers:         27
  Section header string table index: 26
$ file bash-sparc_sparcv9
bash-sparc_sparcv9: ELF 32-bit MSB executable, SPARC32PLUS, V8+ Required, total store ordering, version 1 (SYSV), dynamically linked, interpreter /lib/ld-linux.so.2, for GNU/Linux 2.6.18, BuildID[sha1]=b3a5e202d1abbf480ac690052b0a51f8ce20c8b2, stripped
```
## x86_64 
```
$ readelf -h bash-x86_64
 
ELF Header:
  Magic:   7f 45 4c 46 02 01 01 00 00 00 00 00 00 00 00 00 
  Class:                             ELF64
  Data:                              2's complement, little endian
  Version:                           1 (current)
  OS/ABI:                            UNIX - System V
  ABI Version:                       0
  Type:                              DYN (Position-Independent Executable file)
  Machine:                           Advanced Micro Devices X86-64
  Version:                           0x1
  Entry point address:               0x31dc0
  Start of program headers:          64 (bytes into file)
  Start of section headers:          1388016 (bytes into file)
  Flags:                             0x0
  Size of this header:               64 (bytes)
  Size of program headers:           56 (bytes)
  Number of program headers:         13
  Size of section headers:           64 (bytes)
  Number of section headers:         32
  Section header string table index: 31
$ file bash-x86_64
bash-x86_64: ELF 64-bit LSB pie executable, x86-64, version 1 (SYSV), dynamically linked, interpreter /lib64/ld-linux-x86-64.so.2, BuildID[sha1]=9c4cb71fe5926100833643a8dd221ffb879477a5, for GNU/Linux 3.2.0, stripped
```

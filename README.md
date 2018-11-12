# jos-xv6-macOS

MIT 6.828: https://pdos.csail.mit.edu/6.828/

Run jos and xv6 on macOS.

## Requirements

- Install Homebrew

  ```shell
  /usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
  ```

- Install `qemu`

  ```shell
  brew install qemu
  ```

- Install `i386-elf-gcc` and `i386-jos-elf-gdb`

  ```shell
  brew tap liudangyi/i386-jos-elf-gcc
  brew install i386-jos-elf-gcc i386-jos-elf-gdb
  ```

## Source Code

```shell
git clone https://pdos.csail.mit.edu/6.828/2018/jos.git
git clone git://github.com/mit-pdos/xv6-public.git
```

# jos-xv6-macOS

MIT 6.828: https://pdos.csail.mit.edu/6.828/

Run jos and xv6 on macOS.

## Requirements

- Homebrew: https://brew.sh/

  - Install qemu

    ```shell
    brew install qemu
    ```

- MacPorts: https://www.macports.org/

  - Install `i386-elf-gcc`

    ```shell
    sudo port -v selfupdate
    sudo port install i386-elf-gcc
    ```

## Source Code

```shell
git clone https://pdos.csail.mit.edu/6.828/2018/jos.git
git clone git://github.com/mit-pdos/xv6-public.git
```

## Modify for macOS

Replace all `i386-jos-elf` in the files (`jos/GNUmakefile` and `xv6-public/Makefile`) with `i386-elf` .

## Run

Use qemu.

```shell
qemu-system-i386 -serial mon:stdio -hdb fs.img xv6.img -smp 1 -m 512
```


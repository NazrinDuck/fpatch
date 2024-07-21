# fpatch

A bash script for quickly patchelf by using fzf

To use it, please move fpatch to one of your $PATH first.

Example:

```
mv ./fpatch ~/.local/bin
```

## prerequists

- [fzf](https://github.com/junegunn/fzf)

- [glibc-all-in-one](https://github.com/matrix1001/glibc-all-in-one)

  > and set environment variable $GLIBC=/home/user/glibc-all-in-one

- (suggesting) [tmux](https://github.com/tmux/tmux)

## Usage

```
fpatch [option]... FILE
```

example:

```
fpatch ./a.out # choose libc in fzf
fpatch -f -t ./a.out # choose all libc in fzf --tmux and download it if you don't have
fpatch -h / fpatch --help # for more help
```

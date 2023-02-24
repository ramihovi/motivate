# Motivate

[![Join the chat at https://gitter.im/pymotivate/Lobby](https://badges.gitter.im/pymotivate/Lobby.svg)](https://gitter.im/pymotivate/Lobby?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)

![Motivate](motivate.png)

<br/>

A simple script to print random motivational quotes. Highly influenced by linux command [fortune](https://en.wikipedia.org/wiki/Fortune_(Unix)).

Forked from <https://github.com/mubaris/motivate> (in order to add an option
for a custom data directory).

## Features
* Colored Output
* Supports `bash` and `zsh`
* Custom data (quote) directory

## Requirements

* git
* python 3x

## Installation

### Global install with sudo (Linux)

```sh
$ git clone https://github.com/ramihovi/motivate.git
$ cd motivate/motivate
$ sudo ./install.sh
```

zsh users should replace `.bashrc` with `.zshrc`.

### User install into home directory

If you have no root privilege, or don't want to install motivate globally
(e.g. install in a Qubes OS app vm), you can install this way:

```sh
$ git clone https://github.com/ramihovi/motivate.git
$ cd motivate
$ test -d ~/bin || mkdir ~/bin
$ ln -s $PWD/motivate.py ~/bin/motivate
$ # optional alias:
$ echo "alias motivate='motivate --datadir $PWD/data'" >> [your alias file]
$ source [your alias file]
```

Please note: you must have "~/bin" in PATH environment variable.

### Windows

* Custom data directory option probably doesn't work in Windows (I have no
  Windows machine for testing.)

## Update Database

```sh
$ cd [cloned repo]
$ git pull
```

## Usage

### Normal (global) install or with optional alias added

```sh
$ motivate
```

### User install into home directory

```sh
$ motivate --datadir [path to data directory]
$ # e.g.
$ motivate --datadir /home/user/Git/motivate/motivate/data
$ # with the optional alias:
$ motivate
```

## Contribution

Go to <https://github.com/mubaris/motivate>.


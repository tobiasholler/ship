# ship

Short for <b>sh</b>ell cl<b>ip</b>board.

Sort of a shared clipboard for SSH client and server.

### Copy a file form server to client
#### Server
```sh
$ ship shelf file.zip
```
#### Client
```sh
$ ship download user@server file.zip
```

### Copy a file form client to server
#### Client
```sh
$ ship upload username@wornas file.zip
```
#### Server
```sh
$ ship unshelf file.zip
```

The shelf is so to say the servers clipboard. The client can upload and download from and to it.
Also works with with folders. Also supports bookmarks from `~/.ssh/config`.

## Installation

```sh
git clone --depth=1 https://github.com/tobiasholler/ship
sudo cp ship/ship /usr/bin
sudo chown root:root /usr/bin/ship
```
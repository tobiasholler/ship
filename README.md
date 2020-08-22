# ship

Short for <b>sh</b>ell cl<b>ip</b>board.

Sort of a clipboard for ssh client and server.

### Copy a file form server to client
#### Server
```sh
$ sshclip shelf file.zip
```
#### Client
```sh
$ sshclip download user@server file.zip
```

### Copy a file form client to server
#### Client
```sh
$ sshclip upload username@wornas file.zip
```
#### Server
```sh
$ sshclip unshelf file.zip
```

The shelf is so to say the servers clipboard. The client can upload and download from and to it.
Also works with with folders. Also supports bookmarks from `~/.ssh/config`.
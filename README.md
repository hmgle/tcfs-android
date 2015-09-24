## Tcfs for Android

TCFS, a Lightweight Network File System.

Tcfs-android is the tcfs server for Android.


## How to use?

- Server

TODO

- Client

```
sudo apt-get install libfuse-dev
git clone https://github.com/tcfs/tcfs.git
cd tcfs
mkdir mountpoint
make
# 192.168.0.100 is the server IP address
./tcfs --server 192.168.0.100 mountpoint
ls -shal mountpoint
# access mountpoint
# ...
# unmount tcfs
fusermount -u mountpoint
# or sudo umount mountpoint
```

## Protocol

[TCFS protocol](https://github.com/tcfs/tcfs/blob/master/protocol.adoc)

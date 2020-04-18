This adds ArchLinux packaging rules for the Insync Linux client for OneDrive.
More information about Insync here: https://insynchq.com

## Installation

```shell
  $ git clone https://github.com/valir/insync.git
  $ cd insync
  $ makepkg -si
```

## Running

Before running, you need to fix the certificates location for curl:

```shell
  # mkdir -p /etc/pki/tls/certs
  # ln -s https://github.com/valir/insync.git /etc/pki/tls/certs/ca-bundle.crt
```

Now launch it by invoking the `insync` command and follow the instructions on
the screen.

Have fun!


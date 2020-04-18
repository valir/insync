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

## File manager integration

The Insync web site provides several "Packages" containing configurations for
many Linux file managers. I personnally use Dolphin so I picked-up that one.
Just extract that RPM somewhere on your disk, then just copy the files to the
correct location, using the directory tree from the extracted location. You
may need to create part of those destination paths.

The Dolphin file integration adds a menuitem "Insync" on the right click menu
of the locally synced file. It contains a single entry named "View on web"
wich fires the default browser then points it to the enterprise sharepoint
page for that file.

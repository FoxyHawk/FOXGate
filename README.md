# FOXGate

## Description

FOX stand for :
- Fast : programming priorities (secure & portable > readability > raw performances)
- Open : open source project
- Xperimental : don't expect production ready

Lan gate mainly targeted at Lan parties or more professional events.

Status : designing...
```
 ---------------    -------------
| frontend.conf |--| frontend.py |
 ---------------    -------------
                         |
 ----------          ---------       ------------     ----------------
| net.conf |--------| main.py |-----| checker.py |---| local database |
 ----------          ---------       ------------  |  ----------------
                      |     |                      |
               ---------   ----------              |  -----------------
              | dhcp.py | | ipset.py |             --| other databases |
               ---------   ----------                 -----------------
```

## Development Environment

### Programming Languages

- Python3

### Modules

- `Argparse`
- `Curses`        (net.conf creator)
- `Ipaddr`
- `Logging`
- `Multiprocess`
- `Netaddr`
- `Simplejson`    (\*.conf)
- `Web2py`        (frontend)

### Systems

| OS     | Version | Other      |
| :----- | :------ | :--------- |
| Debian | Stable  | Baremetal  |
| Debian | Stable  | VirtualBox |

### Install

Install/Update packages :
```
apt-get update
apt-get install ipset python3 python3-pip
```

Install via pip needed modules :
```
python3 -m pip install argparse ipaddr multiprocess netaddr simplejson
```

Install `web2py` :
TODO

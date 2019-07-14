# labo-container-connect

connect script for labo-container

```bash
INTERFACE_NAME=eno1 ~/labo-connect/bin/connect
```

###### Table of Contents

- [Requirements](#Requirements)
- [Usage](#Usage)
- [License](#License)


## Requirements

- Docker version 18.09.7, build 2d0083d657


## Usage

```bash
INTERFACE_NAME=eno1 ~/labo-connect/bin/connect
```

- INTERFACE_NAME : network interface for detect ip address

### connect without image update

```bash
INTERFACE_NAME=eno1 ~/labo-connect/bin/connect --without-update
```

### Install

to install labo-connect, clone this repository into your scripts directory

```bash
git clone https://github.com/getto-systems/labo-connect.git /path/to/scripts/labo-connect
```


## License

labo-container-connect is licensed under the [MIT](LICENSE) license.

Copyright &copy; since 2017 shun@getto.systems

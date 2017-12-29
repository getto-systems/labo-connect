# labo-connect

start labo server script for getto/labo

```bash
labo <USER_NAME>
```

###### Table of Contents

- [Requirements](#requirements)
- [Usage](#usage)


<a id="requirements"></a>
## Requirements

- Docker version 17.09.0-ce


<a id="usage"></a>
## Usage

to install labo-connect, clone this repository into your scripts directory

```bash
git clone https://github.com/getto-systems/labo-connect.git /path/to/scripts/labo-connect
```

### Setup Volumes

labo script mount volumes

- apps : mount to /apps
- home : mount to /home/USER_NAME

setup apps and home with docker-sync

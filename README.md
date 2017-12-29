# labo-connect

start script for labo-server([getto/labo](https://github.com/getto-systems/labo))

```bash
labo <USER_NAME>
```

###### Table of Contents

- [Requirements](#requirements)
- [Usage](#usage)
- [License](#license)


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

setup apps and home with [docker-sync](https://github.com/EugenMayer/docker-sync)

```bash
docker-sync start
```

example of docker-sync.yml:

```yaml
version: "2"

options:
  verbose: true
syncs:
  apps:
    sync_userid: '1000'
    src: './apps'
    sync_excludes: []
  home:
    sync_userid: '1000'
    src: './dotfiles'
    sync_excludes: []
```


<a id="license"></a>
## License

labo-connect is licensed under the [MIT](LICENSE) license.

Copyright &copy; since 2017 shun@getto.systems

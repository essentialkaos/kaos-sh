## [kaos.sh](https://kaos.sh)

`kaos.sh` provides simple URL's for working with ESSENTIAL KAOS repositories on GitHub, Travis CI and Coveralls.

### Routing rules

```perl
kaos.sh/{project}                  → github.com/essentialkaos/{project}
kaos.sh/{project}.zip              → github.com/essentialkaos/{project}/archive/master.zip
kaos.sh/{project}.tar.gz           → github.com/essentialkaos/{project}/archive/master.tar.gz
kaos.sh/{project}/{path}           → raw.githubusercontent.com/essentialkaos/{project}/master/{path}
kaos.sh/{project}/{commit}.zip     → github.com/essentialkaos/{project}/archive/{commit}.zip
kaos.sh/{project}/{commit}.tar.gz  → github.com/essentialkaos/{project}/archive/{commit}.tar.gz
kaos.sh/{project}/{version}.zip    → github.com/essentialkaos/{project}/archive/{version}.zip
kaos.sh/{project}/{version}.tar.gz → github.com/essentialkaos/{project}/archive/{version}.tar.gz
kaos.sh/{project}/w/{name}         → github.com/essentialkaos/{project}/wiki/{name}
kaos.sh/{project}/p/{id}           → github.com/essentialkaos/{project}/pull/{name}
kaos.sh/{project}/i/{id}           → github.com/essentialkaos/{project}/issue/{name}
kaos.sh/{project}/r/{tag}          → github.com/essentialkaos/{project}/releases/tag/{tag}
kaos.sh/g/{project}.{tag}          → godoc.org/pkg.re/essentialkaos/{project}.{tag}
kaos.sh/t/{project}                → travis-ci.com/essentialkaos/{project}
kaos.sh/c/{project}                → coveralls.io/github/essentialkaos/{project}
```

### Usage examples

```bash
# Download the latest stable version of KAOSv script
wget https://kaos.sh/kaosv/SOURCES/kaosv
```

```bash
# Download the latest version of RPMBuilder sources as .tar.gz file
curl -o rpmbuilder.tgz https://kaos.sh/rpmbuilder.tar.gz
```

```bash
# Download version 2.2.1 of RPMBuilder sources as .zip file
curl -o rpmbuilder-2.2.1.zip https://kaos.sh/rpmbuilder/v2.2.1.zip
```

```bash
# Pack ek package sources using GoPack without utility installation
bash <(curl -fsSL https://kaos.sh/gopack/SOURCES/gopack) -t v10.0.1 pkg.re/essentialkaos/ek.v10
```

```bash
# Open page of SSLScan repository in Firefox
firefox https://kaos.sh/sslscan
```

```bash
# Open wiki page with RPMBuilder article in Firefox
firefox https://kaos.sh/rpmbuilder/w/Automatic-SHA-512-checksum-generation
```

### License

[EKOL](https://essentialkaos.com/ekol)

<p align="center"><a href="https://essentialkaos.com"><img src="https://gh.kaos.st/ekgh.svg"/></a></p>

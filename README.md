## [kaos.sh](https://kaos.sh)

`kaos.sh` provides simple URL's for working with ESSENTIAL KAOS repositories on GitHub.

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
```

### Examples

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
# Open page of SSLScan repository in Firefox
firefox https://kaos.sh/sslscan
```

### License

[EKOL](https://essentialkaos.com/ekol)

<p align="center"><a href="https://essentialkaos.com"><img src="https://gh.kaos.st/ekgh.svg"/></a></p>

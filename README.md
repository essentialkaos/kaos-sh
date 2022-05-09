## [kaos.sh](https://kaos.sh)

`kaos.sh` provides simple URL's for working with ESSENTIAL KAOS repositories on GitHub, Coveralls and Docker Hub.

### Routing rules

```perl
kaos.sh/{project}                  → github.com/essentialkaos/{project}#readme
kaos.sh/{project}.git              → github.com/essentialkaos/{project}.git
kaos.sh/{project}:{id}             → github.com/essentialkaos/{project}/{pull|issue}/{id}
kaos.sh/{project}:{branch}         → github.com/essentialkaos/{project}/tree/{branch}#readme
kaos.sh/{project}.zip              → github.com/essentialkaos/{project}/archive/master.zip
kaos.sh/{project}.tar.gz           → github.com/essentialkaos/{project}/archive/master.tar.gz
kaos.sh/{project}/{path}           → raw.githubusercontent.com/essentialkaos/{project}/master/{path}
kaos.sh/{project}/:{branch}/{path} → raw.githubusercontent.com/essentialkaos/{project}/{branch}/{path}
kaos.sh/{project}/{commit}.zip     → github.com/essentialkaos/{project}/archive/{commit}.zip
kaos.sh/{project}/{commit}.tar.gz  → github.com/essentialkaos/{project}/archive/{commit}.tar.gz
kaos.sh/{project}/{version}.zip    → github.com/essentialkaos/{project}/archive/{version}.zip
kaos.sh/{project}/{version}.tar.gz → github.com/essentialkaos/{project}/archive/{version}.tar.gz
kaos.sh/{project}/w/{name}         → github.com/essentialkaos/{project}/wiki/{name}
kaos.sh/{project}/p/{id}           → github.com/essentialkaos/{project}/pull/{id}
kaos.sh/{project}/i/{id}           → github.com/essentialkaos/{project}/issue/{id}
kaos.sh/{project}/r/{tag}          → github.com/essentialkaos/{project}/releases/tag/{tag}
kaos.sh/a/{project}                → github.com/essentialkaos/{project}/actions
kaos.sh/b/{project}                → codebeat.co/projects/github-com-essentialkaos-{project}-master
kaos.sh/b/{uuid}.svg               → codebeat.co/badges/{uuid}
kaos.sh/c/{project}                → coveralls.io/github/essentialkaos/{project}
kaos.sh/c/{project}.svg            → coveralls.io/repos/github/essentialkaos/{project}/badge.svg
kaos.sh/d/{project}                → hub.docker.com/r/essentialkaos/{project}
kaos.sh/g/{project}                → pkg.go.dev/github.com/essentialkaos/{project}
kaos.sh/r/{project}                → goreportcard.com/report/github.com/essentialkaos/{project}
kaos.sh/r/{project}.svg            → goreportcard.com/badge/github.com/essentialkaos/{project}
kaos.sh/p/{project}                → github.com/essentialkaos/{project}/pkgs/container/{project}
kaos.sh/v/{project}.svg            → github-readme-stats.vercel.app/api/pin/?username=essentialkaos&repo={project}
kaos.sh/w/{project}/{workflow}     → github.com/essentialkaos/{project}/actions/workflows/{workflow}.yml
kaos.sh/w/{project}/{workflow}.svg → github.com/essentialkaos/{project}/actions/workflows/{workflow}.yml/badge.svg
```

### Usage examples


```html
<p align="center">
  <a href="https://kaos.sh/g/app"><img src="https://gh.kaos.st/godoc.svg" alt="PkgGoDev" /></a>
  <a href="https://kaos.sh/w/app/ci"><img src="https://kaos.sh/w/app/ci.svg" alt="GitHub Actions CI Status" /></a>
  <a href="https://kaos.sh/r/app"><img src="https://kaos.sh/r/app.svg" alt="GoReportCard" /></a>
  <a href="https://kaos.sh/c/app"><img src="https://kaos.sh/c/app.svg" alt="Coverage Status" /></a>
  <a href="https://kaos.sh/b/app"><img src="https://kaos.sh/b/caf0febf-26ae-467c-8237-a6561966d70e.svg" alt="Codebeat badge" /></a>
  <a href="https://kaos.sh/w/app/codeql"><img src="https://kaos.sh/w/app/codeql.svg" alt="GitHub Actions CodeQL Status" /></a>
  <a href="#license"><img src="https://gh.kaos.st/apache2.svg"></a>
</p>
```

```markdown
### Build Status

| Branch | Status |
|--------|----------|
| `master` | [![CI](https://kaos.sh/w/app/ci.svg?branch=master)](https://kaos.sh/w/app/ci?query=branch:master) |
| `develop` | [![CI](https://kaos.sh/w/app/ci.svg?branch=develop)](https://kaos.sh/w/app/ci?query=branch:develop) |
```

```bash
# Clone repository
git clone https://kaos.sh/kaos-repo.git
# or
git clone https://kaos.sh/kaos-repo
```

```bash
# Download the latest stable version of KAOSv script
wget https://kaos.sh/kaosv/SOURCES/kaosv
# Download unstable version (from develop branch) of KAOSv script
wget https://kaos.sh/kaosv/:develop/SOURCES/kaosv
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
bash <(curl -fsSL https://kaos.sh/gopack/SOURCES/gopack) -t v10.0.1 github.com/essentialkaos/ek
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

[Apache License, Version 2.0](https://www.apache.org/licenses/LICENSE-2.0)

<p align="center"><a href="https://essentialkaos.com"><img src="https://gh.kaos.st/ekgh.svg"/></a></p>

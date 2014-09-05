![](https://nodesecurity.io/img/nodesecurity.png)

Node Security Project **Command Line Tools**

## Badgers
[![Dependency Status](https://david-dm.org/nodesecurity/nsp.png)](https://david-dm.org/nodesecurity/nsp)

## Installation

Through npm:
```bash
npm i nsp -g
```

Through GitHub:
```bash
git clone git@github.com:nodesecurity/nsp.git
cd nsp
npm link
```


## `nsp audit-shrinkwrap`
Takes an existing npm-shrinkwrap.json file and submits it for validation to [nodesecurity.io](https://nodesecurity.io/)

**Example:**

```bash
$ nsp audit-shrinkwrap
Name     Installed  Patched  Vulnerable Dependency
connect    2.7.5    >=2.8.1  nodesecurity-jobs > kue > express
```

## `nsp audit-package`
Takes an existing package.json file and submits it for validation to [nodesecurity.io](https://nodesecurity.io/)

**Example:**

```bash
$ nsp audit-package
Name     Installed  Patched  Vulnerable Dependency
connect    2.7.5    >=2.8.1  nodesecurity-jobs > kue > express
```


## TODO

- [ ] Make tests first!
- [ ] Make the review of each dependency work as a stream, so things like https://github.com/nodesecurity/nsp/issues/11 don't happen
- [ ] Contribute to celeri and do a major code refactor and fix of issues
- [ ] Finish lib/nspStream.js to enable https://github.com/nodesecurity/nsp/issues/6
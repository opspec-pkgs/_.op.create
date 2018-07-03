[![Build Status](https://travis-ci.org/opspec-pkgs/_.op.create.svg?branch=master)](https://travis-ci.org/opspec-pkgs/_.op.create)

# Problem statement

internal op for opspec-pkgs/maintainers which automates creation of an official op.

includes:
- creation of github repo
- granting [opspec-pkgs/maintainers team](https://github.com/orgs/opspec-pkgs/teams/maintainers/members) admin permissions
- cloning github repo
- generation of op.yml
- running [bootstrap](https://github.com/opspec-pkgs/_.pkg.bootstrap)


# Format

the op uses [![opspec 0.1.6](https://img.shields.io/badge/opspec-0.1.6-brightgreen.svg?colorA=6b6b6b&colorB=fc16be)](https://opspec.io/0.1.6) definition format

# Example usage

## Install

```shell
opctl op install github.com/opspec-pkgs/_.op.create#3.0.0
```

## Run

```
opctl run github.com/opspec-pkgs/_.op.create#3.0.0
```

## Compose

```yaml
op:
  ref: github.com/opspec-pkgs/_.op.create#3.0.0
  inputs:
    description:
    githubAccessToken:
    githubUsername:
    name:
    # params w/ default
    srcDir:
  outputs:
    srcDir:
```

# Support

join us on
[![Slack](https://opctl-slackin.herokuapp.com/badge.svg)](https://opctl-slackin.herokuapp.com/)
or
[open an issue](https://github.com/opspec-pkgs/_.op.create/issues)

# Releases

releases are versioned according to
[![semver 2.0.0](https://img.shields.io/badge/semver-2.0.0-brightgreen.svg)](http://semver.org/spec/v2.0.0.html)
and [tagged](https://git-scm.com/book/en/v2/Git-Basics-Tagging); see
[CHANGELOG.md](CHANGELOG.md) for release notes

# Contributing

see
[project/CONTRIBUTING.md](https://github.com/opspec-pkgs/project/blob/master/CONTRIBUTING.md)

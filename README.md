[![build](https://github.com/opspec-pkgs/_.op.create/actions/workflows/build.yml/badge.svg)](https://github.com/opspec-pkgs/_.op.create/actions/workflows/build.yml)


# Problem statement

internal op for opspec-pkgs/maintainers which automates creation of an official op.

includes:
- creation of github repo
- granting [opspec-pkgs/maintainers team](https://github.com/orgs/opspec-pkgs/teams/maintainers/members) admin permissions
- cloning github repo
- generation of op.yml
- running [bootstrap](https://github.com/opspec-pkgs/_.pkg.bootstrap)


# Example usage

## Visualize

```shell
opctl ui github.com/opspec-pkgs/_.op.create#4.0.1
```

## Run

```
opctl run github.com/opspec-pkgs/_.op.create#4.0.1
```

## Compose

```yaml
op:
  ref: github.com/opspec-pkgs/_.op.create#4.0.1
  inputs:
    description:  # 👈 required; provide a value
    githubAccessToken:  # 👈 required; provide a value
    githubUsername:  # 👈 required; provide a value
    name:  # 👈 required; provide a value
  ## uncomment to override defaults
  #   srcDir: .
  outputs:
    srcDir:
```

# Support

join us on
[![Slack](https://img.shields.io/badge/slack-opctl-E01563.svg)](https://join.slack.com/t/opctl/shared_invite/zt-51zodvjn-Ul_UXfkhqYLWZPQTvNPp5w)
or
[open an issue](https://github.com/opspec-pkgs/_.op.create/issues)

# Releases

releases are versioned according to
[![semver 2.0.0](https://img.shields.io/badge/semver-2.0.0-brightgreen.svg)](http://semver.org/spec/v2.0.0.html)
and [tagged](https://git-scm.com/book/en/v2/Git-Basics-Tagging); see
[CHANGELOG.md](CHANGELOG.md) for release notes

# Contributing

see
[project/CONTRIBUTING.md](https://github.com/opspec-pkgs/project/blob/main/CONTRIBUTING.md)

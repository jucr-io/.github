![JUCR Logo](https://uploads-ssl.webflow.com/6127780862f49c42bf93addc/6238c2aa8fdf0b02e4898939_JUCR_Logo_Combined.svg) <!-- .element height="50%" width="50%" -->

# JUCR's .github

[![Code Analysis](https://github.com/jucr-io/.github/actions/workflows/ci.yml/badge.svg)](https://github.com/jucr-io/.github/actions/workflows/ci.yml)

# Overview

This repository exists to share Github templates and configuration with other
repositories within the [`JUCR`](https://github.com/jucr-io)
organization.

**This repository is public**. It needs to be public for other repositories to
be able to leverage the templates that it provides.

The approach was taken from=
[this help page](https://help.github.com/en/github/building-a-strong-community/creating-a-default-community-health-file).
And we will keep expanding on this repositories contents!

## Semantic bot Configurations

The default [Semantic Pull Requests](https://github.com/zeke/semantic-pull-requests)
[configuration](.github/semantic.yml) included in this repository can be enabled
by configuring a repository's `.github/stale.yml` to contain the following:

```yaml
titleOnly: true
types:
  - feat
  - fix
  - docs
  - refactor
  - test
  - build
  - ci
  - chore
  - revert
```

## Stalebot Configuration

The default [StaleBot](https://github.com/probot/stale)
[configuration](.github/stale.yml) included in this repository can be enabled
by configuring a repository's `.github/stale.yml` to contain the following:

```yaml
_extends: .github
```

## .gitignore

As default is set to a mix of VisualStudio and MacOS, but you may find other usefull settings [here](https://github.com/github/gitignore)

<!-- markdownlint-disable -->
  <a href="https://jucr.com/">
    <img src="https://github.com/jucr-io/.github/blob/adding-public-info/banner/image_banner.png?raw=true" alt="Project Banner"/>
  </a>
<br/>
<p align="left">
  <a href="https://jucr-io.slack.com">
    <img src="https://upload.wikimedia.org/wikipedia/commons/b/b9/Slack_Technologies_Logo.svg" alt="Slack Community" width="160" height="41"/>
  </a>
</p>
<!-- markdownlint-restore -->

[Last Update](https://img.shields.io/github/last-commit/jucr-io/.github/main)
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

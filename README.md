[![Test Pelles C](https://github.com/Serge3leo/test-pellesc/actions/workflows/test-pellesc.yml/badge.svg)](https://github.com/Serge3leo/test-pellesc/actions/workflows/test-pellesc.yml)

# test-pellesc
Simple test install Pelles C.

The Chocolatey Software, Inc. repository contains versions only up to `12.0.2`,
version `13.01-git-lfs` is installed from this repository (13.01, 23 dec
2025 [https://www.pellesc.se](https://www.pellesc.se).

# Test for long name bug
The `cc` command has an bug in case it is called with an explicit path
that has spaces.

Two options for its bypass are checked:
1. Installation in Pelles C to a directory without spaces on the path. It is set by
   `install-workaround: true`;

2. Setting up environment variables as Short File Name (SFN). It is set by
   `env-workaround: true`;

# Usage
Fork the repository. Create a PR with the name prefixed with `Test...`, where
you can change the parameters `install-workaround` or `env-workaround`. Check
the GitHub Actions protocol.

# Contributing
Issues or PRs are accepted and welcome.

# Disclaimer
Sorry for my best English.  Alas, this file is actually a yandex translation of
[README.ru.md](README.ru.md) with minimal editorial changes.

# License
[BSD-2-Clause © 2025 Сергей Леонтьев (leo@sai.msu.ru).](LICENSE)

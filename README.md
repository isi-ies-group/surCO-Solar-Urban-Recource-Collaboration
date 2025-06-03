# surCO - Solar Urban Resource Collaboration

*surCO* is a data-crowdsourced initiative that aims to quantify the energy yield of vehicle-integrated photovoltaics (VIPV).

## This monorepo

Via submodules, this monorepo contains each individual project. Three main purposes are filled by each one:

- Client side data acquisition: right now, an Android application and configuration files for the beacons that shall be joined to the car surfaces via magnets.
- Server side data storage: a Python web server with an API where users can register, login and the app can post session files. The server may require some specific version of the files, so as to require the client to be up-to-date.
- Post-processing parser for reading the session files. Currently done in Python.

This repo may be considered a long-term reference of the tools used in *surCO*.

## Instructions

If submodules have not already been initialized in the clone command, you may set up this repo by using the helper scripts in `/scripts`. Run:
- Unix-OS: `./scripts/git-setup-submodules`
- Windows: `type .\scripts\git-setup-submodules | cmd`
`
For fetching (updating) the latests changes from each subproject remote, do:
- Unix-OS: `./scripts/git-update-fetch-submodules`
- Windows: `type .\scripts\git-update-fetch-submodules | cmd`

In any case, you can always use each project individually.

## Versions management

Since the project is in early development with a small group of testers, big changes can still be expected. Sub-projects are not expected to enforce a special version management that ensures compatibility. For best results, use the latest commit in `main` or the latest tagged commit, if any.

## License and authors

License is MIT. See `LICENSE`.

Developed by Instrumentation and Systems Integration group, Instituto de Energía Solar.

Copyright © Universidad Politécnica de Madrid. 2024, 2025.

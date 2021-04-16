# Ansible Role: Polychromatic

[![CI](https://github.com/pmikus/ansible-role-polychromatic/actions/workflows/CI.yml/badge.svg)](https://github.com/pmikus/ansible-role-polychromatic/actions/workflows/CI.yml)
[![Reliability Rating](https://sonarcloud.io/api/project_badges/measure?project=pmikus_ansible-role-polychromatic&metric=reliability_rating)](https://sonarcloud.io/dashboard?id=pmikus_ansible-role-polychromatic)
[![Bugs](https://sonarcloud.io/api/project_badges/measure?project=pmikus_ansible-role-polychromatic&metric=bugs)](https://sonarcloud.io/dashboard?id=pmikus_ansible-role-polychromatic)

## Requirements

This role depends on [pmikus.ansible-role-openrazer](https://github.com/pmikus/ansible-role-openrazer).

## Role Variables

Available variables are listed below, along with default values (see `defaults/main.yml`):

    polychromatic_package: "darktable"

Name of package in package repository.

    polychromatic_package_state: "present"

Install package (optionally you can change to "absent" to uninstall).

    darktable_apt_state: "present"

Install APT repository (optionally you can change to "absent" to roll back).

    polychromatic_apt_release_channel: "daily"

APT channel can be one of: "stable" or "daily".

## Dependencies

None

## Example Playbook

    - hosts: localhost
      roles:
        - pmikus.ansible-role-polychromatic

## License

MIT / BSD

## Author Information

This role was created by [Peter Mikus](https://www.linkedin.com/in/petermikus/).

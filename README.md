# levonet.sonarqube-scanner
[![Build Status](https://travis-ci.org/levonet/ansible-sonarqube-scanner.svg?branch=master)](https://travis-ci.org/levonet/ansible-sonarqube-scanner)

An Ansible Role that installs [Sonar Scanner](https://docs.sonarqube.org/display/SCAN/Analyzing+with+SonarQube+Scanner)
on Ubuntu/Debian/RedHat/CentOS/Fedora/Suse Linux and macOS servers.

## Requirements

Requires the `unzip` utility to be installed on the server.

## Role Variables

| Variable                | Description            | Default      |
|-------------------------|------------------------|--------------|
| `sonar_scanner_version` | Version                | `3.3.0.1492` |
| `sonar_scanner_mirror`  | URL | `https://binaries.sonarsource.com/Distribution/sonar-scanner-cli` |
| `sonar_scanner_prefix`  | Installation directory | `/usr/local` |

## Dependencies

- none

## Example Playbook

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
        - role: levonet.sonarqube-scanner
          sonar_scanner_version: "3.2.0.1227"

License
-------

MIT

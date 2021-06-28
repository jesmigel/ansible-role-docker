# ansible-role-docker
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT) 
[![CI](https://github.com/jesmigel/ansible-role-docker/actions/workflows/build.yaml/badge.svg?branch=main)](https://github.com/jesmigel/ansible-role-docker/actions/workflows/build.yaml)

Ansible role used to set up a docker host.

### References
| Name | Comments |
| - | - |
| [Dependencies](https://github.com/jesmigel/ansible-role-common#dependencies) | Deployment Toolchain |
| [Make Commands](https://github.com/jesmigel/ansible-role-common#make-commands) | Deployment Shortcuts |
| [Preflight Steps](https://github.com/jesmigel/ansible-role-common#preflieght-steps) | Pre deployment configuration 
|||

### Tools Installed
| Name | Comments |
| - | - |
| [Docker](https://docs.docker.com/) | Docker is a set of platform as a service products that use OS-level virtualization to deliver software in packages called containers. |
|||

### Tests
- `Lint`: yamllint and ansible-lint. This is automated through Github Actions
- `Functional`: Tested through Vagrant and ESXi. To be added in github actions

### Usage
This repository is used as an ansible role. It can be referenced through a requirements.yaml file.
```yaml
# from github
- src: https://github.com/jesmigel/ansible-role-docker.git
  name: hashicorp
```

The role can be installed through the ansible-galaxy command:
```bash
ansible-galaxy role install -r requirements.yaml -p $ROLE_DIRECTORY
```

### ToDo
1. DevOps CI/CD test
    - Jenkins

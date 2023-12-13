# stephrobert.lynis

[![Maintainer](https://img.shields.io/badge/maintained%20by-stephrobert-e00000?style=flat-square)](https://github.com/stephrobert)
[![License](https://img.shields.io/github/license/stephrobert/ansible-role-openscap?style=flat-square)](https://github.com/stephrobert/ansible-role-openscap/blob/main/LICENSE)
[![Release](https://img.shields.io/github/v/release/stephrobert/ansible-role-openscap?style=flat-square)](https://github.com/stephrobert/ansible-role-openscap/releases)
[![Status](https://img.shields.io/github/workflow/status/stephrobert/ansible-role-openscap/Ansible%20Molecule?style=flat-square&label=tests)](https://github.com/stephrobert/ansible-role-openscap/actions?query=workflow%3A%22Ansible+Molecule%22)
[![Ansible Galaxy](https://img.shields.io/badge/ansible-galaxy-black.svg?style=flat-square&logo=ansible)](https://galaxy.ansible.com/stephrobert/lynis)[![Ansible version](https://img.shields.io/badge/ansible-%3E%3D2.10-black.svg?style=flat-square&logo=ansible)](https://github.com/ansible/ansible)

⭐ Star us on GitHub — it motivates us a lot!

Install Lynis

**Platforms Supported**:

| Platform | Versions |
|----------|----------|
| Debian | bullseye |
| Ubuntu | jammy |

## ⚠️ Requirements

Ansible >= 2.11.

### Ansible role dependencies

None.

## ⚡ Installation

### Install with Ansible Galaxy

```shell
ansible-galaxy install stephrobert.lynis
```

### Install with git

If you do not want a global installation, clone it into your `roles_path`.

```bash
git clone git@github.com:stephrobert/ansible-role-openscap.git  stephrobert.lynis
```

But I often add it as a submodule in a given `playbook_dir` repository.

```bash
git submodule add git@github.com:stephrobert/ansible-role-openscap.git roles/stephrobert.lynis
```

As the role is not managed by Ansible Galaxy, you do not have to specify the
github user account.

### ✏️ Example Playbook

Basic usage is:

```yaml
- hosts: all
  roles:
    - role: stephrobert.lynis
      vars:
        lynis_version: 3.0.9
        scan: false
        
```

## ⚙️ Role Variables

Variables are divided in three types.

The **default vars** section shows you which variables you may
override in your ansible inventory. As a matter of fact, all variables should
be defined there for explicitness, ease of documentation as well as overall
role manageability.

The **context variables** are shown in section below hint you
on how runtime context may affects role execution.

### Default variables
Role default variables from `defaults/main.yml`.

| Variable Name | Value |
|---------------|-------|
| lynis_version | 3.0.9 |
| scan | False |

### Context variables

Those variables from `vars/*.{yml,json}` are loaded dynamically during task
runtime using the `include_vars` module.

Variables loaded from `vars/main.yml`.




## Author Information

none
# kibana

[![Source Code](https://img.shields.io/badge/github-source%20code-blue?logo=github&amp;logoColor=white)](https://github.com/rolehippie/kibana)
[![General Workflow](https://github.com/rolehippie/kibana/actions/workflows/general.yml/badge.svg)](https://github.com/rolehippie/kibana/actions/workflows/general.yml)
[![Readme Workflow](https://github.com/rolehippie/kibana/actions/workflows/readme.yml/badge.svg)](https://github.com/rolehippie/kibana/actions/workflows/readme.yml)
[![Galaxy Workflow](https://github.com/rolehippie/kibana/actions/workflows/galaxy.yml/badge.svg)](https://github.com/rolehippie/kibana/actions/workflows/galaxy.yml)
[![License: Apache-2.0](https://img.shields.io/github/license/rolehippie/kibana)](https://github.com/rolehippie/kibana/blob/master/LICENSE)
[![Ansible Role](https://img.shields.io/badge/role-rolehippie.kibana-blue)](https://galaxy.ansible.com/rolehippie/kibana)

Ansible role to install and configure a Kibana dashboard.

## Sponsor

Building and improving this Ansible role have been sponsored by my current and previous employers like **[Cloudpunks GmbH](https://cloudpunks.de)** and **[Proact Deutschland GmbH](https://www.proact.eu)**.

## Table of content

- [Requirements](#requirements)
- [Default Variables](#default-variables)
  - [kibana_elasticsearch_hosts](#kibana_elasticsearch_hosts)
  - [kibana_elasticsearch_preserve_host](#kibana_elasticsearch_preserve_host)
  - [kibana_group](#kibana_group)
  - [kibana_keyring](#kibana_keyring)
  - [kibana_major_version](#kibana_major_version)
  - [kibana_server_base_path](#kibana_server_base_path)
  - [kibana_server_name](#kibana_server_name)
  - [kibana_server_version](#kibana_server_version)
  - [kibana_user](#kibana_user)
- [Discovered Tags](#discovered-tags)
- [Dependencies](#dependencies)
- [License](#license)
- [Author](#author)

---

## Requirements

- Minimum Ansible version: `2.10`


## Default Variables

### kibana_elasticsearch_hosts

#### Default value

```YAML
kibana_elasticsearch_hosts: []
```

### kibana_elasticsearch_preserve_host

#### Default value

```YAML
kibana_elasticsearch_preserve_host: false
```

### kibana_group

Name of the group owning Kibana

#### Default value

```YAML
kibana_group: kibana
```

### kibana_keyring

Path for the repository keyring

#### Default value

```YAML
kibana_keyring: /usr/share/keyrings/elastic-archive-keyring.gpg
```

### kibana_major_version

Major version built via server version variable

#### Default value

```YAML
kibana_major_version: "{{ kibana_server_version.split('.')[0] }}"
```

### kibana_server_base_path

When this setting's value is true Kibana uses the hostname specified in server host

### kibana_server_name

Name of the server

#### Default value

```YAML
kibana_server_name: '{{ ansible_hostname }}'
```

### kibana_server_version

Version of Kibana that gets installed

#### Default value

```YAML
kibana_server_version: '7.8'
```

### kibana_user

Name of the user owning Kibana

#### Default value

```YAML
kibana_user: kibana
```

## Discovered Tags

**_kibana_**


## Dependencies

- None

## License

Apache-2.0

## Author

[Thomas Boerger](https://github.com/tboerger)
